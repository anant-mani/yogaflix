# Yogaflix pose artwork brief

Copy-paste material for generating pose illustrations with ChatGPT / Gemini.
Do everything in ONE chat session so the style stays consistent.

## Step 1 — set the style (paste this first)

> I'm creating a set of 19 yoga pose illustrations for a mobile app with a dark
> background. Requirements for EVERY image, keep them identical across the set:
>
> - Minimal elegant illustration of ONE person in a yoga pose
> - [YOUR STYLE CHOICE — e.g. "flat vector illustration" / "soft watercolor" /
>   "ink brush drawing" / "clean line art with subtle fills"]
> - Single color palette: warm amber/cream (#f0c987) with soft orange accents (#e79a5f)
> - Fully TRANSPARENT background — no backdrop, no floor, no mat, no shadow
> - Square 1:1, figure centered, filling about 80% of the frame
> - Same character in every image: relaxed adult, simple features, calm expression
> - Head upright, gaze forward (they're watching TV while practising)
> - No text, no watermark, no border
>
> I'll ask for the poses one at a time. Keep the character, style, line weight,
> and scale identical to the previous images every time.

## Step 2 — the poses (one message each: "Same character, same style: …")

| # | Filename | Pose prompt |
|---|----------|-------------|
| 1 | `easy.png` | Easy Pose (Sukhasana) — sitting cross-legged, hands resting on knees, spine tall, gaze forward |
| 2 | `thunder.png` | Thunderbolt (Vajrasana) — kneeling, sitting back on heels, hands on thighs, spine tall |
| 3 | `sidebend.png` | Seated Side Bend — cross-legged, one arm reaching up and over to the side, other hand on floor |
| 4 | `staff.png` | Staff Pose (Dandasana) — sitting with both legs straight ahead, feet flexed, palms on floor beside hips, spine tall |
| 5 | `butterfly.png` | Butterfly (Baddha Konasana) — seated, soles of feet together, knees dropped out, hands holding feet |
| 6 | `twist.png` | Seated Twist (Ardha Matsyendrasana) — seated, one knee up, torso gently twisted, looking over shoulder-ish but head up |
| 7 | `cowface.png` | Cow-Face Arms (Gomukhasana) — seated cross-legged, one arm reaching over shoulder from above, the other from below behind the back, hands clasped |
| 8 | `wideleg.png` | Wide-Leg Seat (Upavistha Konasana) — seated, legs open wide, feet flexed, chest lifted, hands on floor in front |
| 9 | `pigeon.png` | Pigeon Pose (Eka Pada Kapotasana) — front shin folded forward on floor, back leg extended straight behind, chest lifted, gaze forward |
| 10 | `lunge.png` | Low Lunge (Anjaneyasana) — one foot forward in a lunge, back knee on floor, chest lifted, gaze forward |
| 11 | `catcow.png` | Cat–Cow (Marjaryasana) — on hands and knees, back gently arched, head lifted looking forward |
| 12 | `sphinx.png` | Sphinx Pose (Salamba Bhujangasana) — lying on belly, propped on forearms, chest lifted, gaze forward |
| 13 | `child.png` | Child's Pose (Balasana) — kneeling folded forward, forehead down, arms extended forward on floor |
| 14 | `meditate.png` | Meditation Seal (Anjali Mudra) — seated cross-legged, palms together at the heart, eyes soft, spine tall |
| 15 | `ankleFB.png` | Ankle Point & Flex — Staff Pose (legs straight ahead, palms beside hips) with toes pointing forward, suggesting foot movement |
| 16 | `ankleLR.png` | Ankle Sway — Staff Pose with both feet tilted to one side, suggesting side-to-side foot movement |
| 17 | `ankleRot.png` | Ankle Circles — Staff Pose with feet mid-rotation, suggesting circular foot movement |
| 18 | `kneehug.png` | Knee Hug (Pawanmuktasana seated) — seated with one leg straight, other knee hugged to chest with both arms, spine tall |
| 19 | `reachup.png` | Kneeling Reach Up (Parvatasana in Vajrasana) — kneeling on heels, arms stretched straight overhead, fingers interlaced, palms facing the sky |

## Step 3 — hand off

Put the files in a folder (any folder) and tell Claude where they are.
Renaming to the filenames above is helpful but optional.

Claude will then: optimize/compress them (WebP), wire them into the app in
place of the code-drawn silhouettes, keep the mat line + animated arrows for
the three ankle drills, and redeploy.

## Tips

- Generate 1 pose first, iterate until you LOVE the style, then do the rest.
- If a result drifts off-style, reply "redo in exactly the same style as the
  first image" (or attach the first image as reference).
- Transparent background is the most commonly ignored instruction — check each
  image, and re-ask if it comes back with a background.
