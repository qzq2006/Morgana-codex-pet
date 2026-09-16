Create one horizontal animation strip for Codex pet `morgana-zorro`, state `idle`.

Use the attached canonical base for identity. Use the attached layout guide only for slot count, spacing, centering, and padding; do not draw the guide.

Output exactly 6 full-body frames in one left-to-right row on flat pure user-selected #FF00FF. Treat the row as 6 invisible equal-width slots: one centered complete pose per slot, evenly spaced, with no overlap, clipping, empty slots, labels, or borders.

Identity: same pet in every frame: Preserve the existing Morgana pet identity exactly. Zorro is a state-specific Persona apparition only in running, review, and failed: a masked gentleman swordsman in formal attire with a readable Z belt emblem, rendered as a compact high-contrast attached silhouette behind and overlapping Morgana. Keep all other standard states visually identical to the original Morgana pet.. Preserve silhouette, face, proportions, markings, palette, material, style, and props.
Style: Pet-safe sprite: compact full-body mascot, readable in a 192x208 cell, clear silhouette, simple face, stable palette/materials, and crisp edges for chroma-key extraction. Style `auto`: Infer the most appropriate pet-safe style from the user request and reference images, then keep that exact style consistent across every row. User style notes: Match the current clean non-pixel chibi Morgana sprites: black, white, bright blue eyes, yellow scarf, crisp hard-edged forms readable at 59x64..
Animation continuity: keep apparent pet scale and baseline stable within the row unless the state itself intentionally changes vertical position, such as `jumping`. Move the pose within the slot instead of redrawing the pet larger or smaller frame to frame.

State action: Calm but visibly alive low-distraction resting loop: layered breathing, one natural blink, a tiny asymmetric ear response, and delayed tail/scarf follow-through.

State requirements:
- CRITICAL: idle is the low-distraction baseline state and the first frame is also used as the reduced-motion static pet.
- Use only subtle idle motion, but make the micro-motion readable at pet size. Chest and shoulders rise and fall by about 2-3 pixels while the planted feet remain fixed.
- Keep the pet essentially in the same pose, facing direction, silhouette, markings, palette, and prop state across all 6 frames.
- Idle variation must stay calm but still read as animation; do not repeat effectively identical copies across the loop.
- Six-frame performance, left to right:
  - Frame 1: neutral planted pose at the start of an inhale, eyes open.
  - Frame 2: chest and head rise slightly; tail begins to follow one phase late.
  - Frame 3: top of inhale with a half blink and one ear dipping only a tiny amount.
  - Frame 4: eyes briefly closed, shoulders beginning to exhale; the ear is already recovering.
  - Frame 5: body settles lower while the tail and scarf tips gently overshoot in the opposite direction.
  - Frame 6: eyes open and pose returns close to Frame 1, with only a tiny residual tail/scarf lag so the loop closes smoothly.
- Keep the head response slightly later than the chest, and keep the tail and scarf one phase later than the body. Their motion should form a soft delayed S-curve instead of flipping direction together.
- Preserve Morgana's two simple ears, two attached arms and white paws, planted feet, clean curved tail, and two yellow scarf tips in every frame.
- Do not show waving, walking, running, jumping, talking, working, reviewing, emotional reactions, large gestures, item interactions, or new props.
- Feet, base, body, or object anchor should remain planted or nearly planted.
- The first and last frames should be very close visually so the loop feels calm and does not pop.

Clean extraction: crisp opaque edges, safe padding, no scenery, text, guide marks, checkerboard, shadows, glows, motion blur, speed lines, dust, detached effects, stray pixels, or chroma-key colors inside the pet.
