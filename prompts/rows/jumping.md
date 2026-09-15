Create one horizontal animation strip for Codex pet `morgana-zorro`, state `jumping`.

Use the attached canonical base for identity. Use the attached layout guide only for slot count, spacing, centering, and padding; do not draw the guide.

Output exactly 5 full-body frames in one left-to-right row on flat pure user-selected #FF00FF. Treat the row as 5 invisible equal-width slots: one centered complete pose per slot, evenly spaced, with no overlap, clipping, empty slots, labels, or borders.

Identity: same pet in every frame: Preserve the existing Morgana pet identity exactly. Zorro is a state-specific Persona apparition only in running, review, and failed: a masked gentleman swordsman in formal attire with a readable Z belt emblem, rendered as a compact high-contrast attached silhouette behind and overlapping Morgana. Keep all other standard states visually identical to the original Morgana pet.. Preserve silhouette, face, proportions, markings, palette, material, style, and props.
Style: Match the attached current Morgana sprite row exactly: clean flat 2D vector-like shapes, crisp hard edges, minimal shading, small compact body, and the same head-to-body ratio as the existing v2 pet. This is not a redesign. Do not make the head, face, or eyes larger. Do not use painterly rendering, soft 3D lighting, glossy materials, fur texture, gradients, or a toy/figurine look. Keep the official black, white, bright-blue-eye, and yellow-scarf palette. The attached current jumping row is a style/proportion reference only; ignore and correct any magenta fringe visible inside its source sprites. Pure #FF00FF belongs only to the background and must never appear inside Morgana.
Animation continuity: keep apparent pet scale and baseline stable within the row unless the state itself intentionally changes vertical position, such as `jumping`. Move the pose within the slot instead of redrawing the pet larger or smaller frame to frame.

State action: Hover jump loop: anticipation, lift, airborne peak, descent, and settle through body height.

State requirements:
- Show the jump through pose and vertical body position only: anticipation, lift, airborne peak, descent, settle.
- Do not draw ground shadows, contact shadows, drop shadows, oval shadows, landing marks, dust, smears, bounce pads, or motion marks under the pet.
- Keep the background outside the pet perfectly flat chroma key with no darker key-colored patches.

Five-frame motion plan, left to right:
- Frame 1: clear anticipation crouch, body about 4 pixels lower than the resting baseline, knees compressed, ears slightly lowered, tail and scarf still trailing upward.
- Frame 2: rising pose, body about 10 pixels above the resting baseline, legs extending and arms beginning to lift.
- Frame 3: unmistakable airborne apex, body about 22 pixels above the resting baseline, feet clearly lifted, compact readable silhouette; tail and scarf lag below the body.
- Frame 4: descending counterpart to Frame 2, body about 10 pixels above baseline, limbs preparing for contact; tail and scarf remain one phase behind.
- Frame 5: soft landing/settle at the resting baseline, knees slightly compressed and visually close enough to Frame 1 for a smooth loop.
- Keep Morgana's head size, torso width, face, and overall scale identical. Change vertical position and pose, never redraw him larger or smaller.
- Match the current reference row's compact silhouette and facial construction in every frame. The previous large-headed, rounded, painterly interpretation is explicitly forbidden.
- Preserve one continuous jump arc: anticipation -> acceleration -> apex -> descent -> landing. No frame may look like an unrelated standing or waving pose.

Clean extraction: crisp opaque edges, safe padding, no scenery, text, guide marks, checkerboard, shadows, glows, motion blur, speed lines, dust, detached effects, stray pixels, or chroma-key colors inside the pet.
