# Morgana look-direction mechanics

Rows 9–10 contain Morgana only. Zorro remains exclusive to the `failed`, `running`, and `review` standard-state rows.

- Anchor Morgana's feet and lower torso to the same baseline and scale as the original idle pose.
- Lead each direction with the bright blue pupils, then rotate the head and muzzle subtly; ears follow the head and the tail lags slightly.
- Keep the yellow scarf attached and let it follow the turn with a small, coherent offset.
- Never rotate the entire body like a flat card. Preserve a mostly forward torso and use face, eye, ear, and slight shoulder changes.
- `000` up: pupils and muzzle angle upward; ears lift slightly.
- `090` screen-right: pupils, muzzle, and head point toward screen-right; show a little more of Morgana's right-facing side.
- `180` down: pupils and muzzle lower; ears relax slightly.
- `270` screen-left: pupils, muzzle, and head point toward screen-left; show a little more of Morgana's left-facing side.
- Interpolate the 16 directions smoothly clockwise. `337.5` must return naturally toward the neutral/up-facing start.
