Create one horizontal animation strip for Codex pet `morgana-zorro`, state `running`.

Use the attached canonical base for identity. Use the attached layout guide only for slot count, spacing, centering, and padding; do not draw the guide.

Output exactly 6 full-body frames in one left-to-right row on flat pure user-selected #FF00FF. Treat the row as 6 invisible equal-width slots: one centered complete pose per slot, evenly spaced, with no overlap, clipping, empty slots, labels, or borders.

Identity: preserve the existing Morgana pet exactly. Copy Zorro from the attached official Zorro reference: enormous inverted-triangle torso, broad rounded shoulders, oversized black puffed sleeves and fists, narrow ornate black-and-silver corseted body, extremely long thin legs, pointed shoes, small silver bird-beak helmet/mask with yellow eyes, blue neck detail, ornate silver waist emblem, slim rapier, and huge black wing-like cape tails with silver trim. Do not invent or substitute a generic masked gentleman, knight, rogue, pirate, or human-proportioned swordsman. Preserve silhouette, face, proportions, markings, palette, material, style, and props.
Style: Pet-safe sprite: compact full-body mascot, readable in a 192x208 cell, clear silhouette, simple face, stable palette/materials, and crisp edges for chroma-key extraction. Style `auto`: Infer the most appropriate pet-safe style from the user request and reference images, then keep that exact style consistent across every row. User style notes: Match the current clean non-pixel chibi Morgana sprites: black, white, bright blue eyes, yellow scarf, crisp hard-edged forms readable at 59x64..
Animation continuity: keep apparent pet scale and baseline stable within the row unless the state itself intentionally changes vertical position, such as `jumping`. Move the pose within the slot instead of redrawing the pet larger or smaller frame to frame.

State action: Working loop: focused active-task processing, thinking, typing, scanning, or effortful concentration; not literal foot-running, jogging, sprinting, treadmill motion, raised knees, long steps, pumping arms, or directional travel.

State requirements:
- Show the pet actively working or processing, as if running a task: focused posture, busy hands or paws, purposeful bobbing, thinking motion, tool or prop motion only if already part of the pet identity, or other non-locomotion activity.
- Do not show literal foot-running, jogging, sprinting, treadmill motion, raised knees, long steps, pumping arms, directional travel, speed lines, dust clouds, floor shadows, motion trails, or detached motion effects.

Persona Edition action, left to right:
- Make a quiet closed working loop, not a summon or disappearance sequence. Zorro is already fully present directly behind and overlapping Morgana in every frame.
- Lock both characters' feet, lower torso, overall scale, and shared center to the same position in all six frames. Keep Zorro's torso, legs, shoulders, and cape nearly stationary.
- Frame 1: compact ready pose, Zorro's sword held at a low guarded diagonal; Morgana focuses forward.
- Frame 2: raise only Zorro's sword forearm by about 10 degrees; Morgana's eyes begin tracking it.
- Frame 3: raise the sword another 10 degrees; add a tiny shoulder follow-through and a one-frame-late scarf/tail response.
- Frame 4: perform one short controlled diagonal work stroke using the sword arm only; no lunge, scale change, body translation, or silhouette explosion.
- Frame 5: return through the Frame 3 pose.
- Frame 6: return through the Frame 2 pose so the transition back to Frame 1 is very small.
- Preserve Zorro's giant shoulders and fists, tiny beaked yellow-eyed mask, thin long legs, wing-like cape tails, ornate waist, and rapier, but prioritize stable registration and small evenly spaced motion over dramatic action.
- The six poses must read as A-B-C-D-C-B, with Frame 6 adjacent to Frame 1 and no popping at the loop boundary.

Clean extraction: crisp opaque edges, safe padding, no scenery, text, guide marks, checkerboard, shadows, glows, motion blur, speed lines, dust, detached effects, stray pixels, or chroma-key colors inside the pet.
