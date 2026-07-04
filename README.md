# Yogaflix 🧘

**Gentle floor yoga you can do while you watch your favourite show.**

Yogaflix is a tiny, free web app: roll out a mat in front of the TV, pick a session
length, and it guides you through calm seated poses with a soft bell cueing each
change. Every pose keeps your gaze up so you never miss a scene — you just breathe
and watch.

🔗 **Live:** _add your Cloudflare Pages URL here_

## Features

- **10 / 20 / 30 / 40-minute sessions** — pick how long you want to sit.
- **Randomized warm-up → flow → rest arc** — a fresh sequence every time, but always
  eased in and out sensibly (never a deep stretch cold).
- **Illustrated pose figures** — a consistent hand-illustrated character for every
  pose (`art/`, sliced from a single AI-generated sheet), in an energy-friendly
  dark theme.
- **Soft synthesized bell** cues each transition — no audio files, works offline.
- **Breathing pulse** and a screen **wake-lock** so your phone won't sleep on the mat.
- **Local-only personalization** — after a few days of practice it invites you to add
  your name and a custom greeting. Nothing leaves your device; there is no account.

## Tech

One `index.html` plus a folder of pose illustrations (`art/*.webp`) — no build
step, no dependencies, no backend. Sessions, audio, and UI are all generated in
the browser. `poses-sheet.png` is the original artwork sheet the poses were
sliced from.

## Run locally

Just open `index.html` in a browser, or serve the folder:

```bash
python3 -m http.server 4599
# then visit http://localhost:4599
```

## Deploy (Cloudflare Pages)

```bash
npx wrangler pages deploy . --project-name yogaflix
```

Or connect this GitHub repo in the Cloudflare dashboard (Pages → Create → Connect to
Git) with an empty build command and the repo root as the output directory.

## Analytics

Yogaflix supports **Cloudflare Web Analytics** (privacy-friendly, cookieless). To turn
it on:

1. Cloudflare dashboard → **Web Analytics** → **Add a site** → paste your Pages URL.
2. Copy the **token** it gives you.
3. Set `CF_ANALYTICS_TOKEN` near the bottom of `index.html` to that token and redeploy.

Leaving the token empty simply disables the beacon.

## License

[MIT](LICENSE) — free for everyone, everywhere. 🙏
