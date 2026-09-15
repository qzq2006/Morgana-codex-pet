Create one horizontal animation strip for Codex pet `morgana-zorro`, state `failed`.

Use the attached canonical base for identity. Use the attached layout guide only for slot count, spacing, centering, and padding; do not draw the guide.

Output exactly 8 full-body frames in one left-to-right row on flat pure user-selected #FF00FF. Treat the row as 8 invisible equal-width slots: one centered complete pose per slot, evenly spaced, with no overlap, clipping, empty slots, labels, or borders.

Identity: preserve the existing Morgana pet exactly. Copy Zorro from the attached official Zorro reference: enormous inverted-triangle torso, broad rounded shoulders, oversized black puffed sleeves and fists, narrow ornate black-and-silver corseted body, extremely long thin legs, pointed shoes, small silver bird-beak helmet/mask with yellow eyes, blue neck detail, ornate silver waist emblem, slim rapier, and huge black wing-like cape tails with silver trim. Do not invent or substitute a generic masked gentleman, knight, rogue, pirate, or human-proportioned swordsman. Preserve silhouette, face, proportions, markings, palette, material, style, and props.
Style: Pet-safe sprite: compact full-body mascot, readable in a 192x208 cell, clear silhouette, simple face, stable palette/materials, and crisp edges for chroma-key extraction. Style `auto`: Infer the most appropriate pet-safe style from the user request and reference images, then keep that exact style consistent across every row. User style notes: Match the current clean non-pixel chibi Morgana sprites: black, white, bright blue eyes, yellow scarf, crisp hard-edged forms readable at 59x64..
Animation continuity: keep apparent pet scale and baseline stable within the row unless the state itself intentionally changes vertical position, such as `jumping`. Move the pose within the slot instead of redrawing the pet larger or smaller frame to frame.

State action: Blocked/failed loop: slumped or deflated reaction with sad or closed eyes.

State requirements:
- Show failure through slumped pose, drooping ears/limbs, closed or sad eyes, and lower body position.
- Tears, small smoke puffs, or tiny stars are allowed only if attached to or overlapping the pet silhouette and kept inside the same frame slot.
- Do not draw red X marks, floating symbols, detached stars, separated smoke clouds, falling tear drops, dust, or other loose effects.

Persona Edition action, left to right:
- Frame 1 begins with Zorro fully present directly behind and overlapping Morgana, but both already look weakened.
- Frames 2-3 lower Zorro's sword and shoulders while Morgana's ears and posture droop.
- Frames 4-6 fold Zorro's cape and body inward behind Morgana, progressively hiding him through physical occlusion rather than transparency.
- Frame 7 leaves only a small attached portion of Zorro's upper silhouette touching Morgana's shoulder line.
- Frame 8 shows Morgana alone in a settled sad pose, ready to loop back to the initial failed reaction.
- Never use transparent fading, ghost copies, detached fragments, smoke, particles, or glow to depict disappearance.

Clean extraction: crisp opaque edges, safe padding, no scenery, text, guide marks, checkerboard, shadows, glows, motion blur, speed lines, dust, detached effects, stray pixels, or chroma-key colors inside the pet.
