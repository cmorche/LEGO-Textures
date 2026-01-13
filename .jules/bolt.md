## 2025-01-13 - [Asset Optimization]
**Learning:** Found significant savings (~26%) in `LEGO Minifigures/Series 5`. Older series or less prominent assets may be less likely to be optimized than root assets like `header.png`.
**Action:** When looking for optimization candidates, check deeper into specific theme subdirectories if root assets are already optimized.

## 2025-01-05 - Found Unoptimized PNGs
**Learning:** The repository contains several large PNG files (e.g., `Ninjago/Slithra/Slithra Head.png` ~516K) that are not optimized. `optipng` can significantly reduce their size without losing quality.
**Action:** Run `optipng -o7` on large assets to improve download speeds and reduce repository size.
## 2025-12-31 - [Asset Optimization]
**Learning:** This repository consists entirely of static assets with no build system. Performance gains come exclusively from optimizing these assets (e.g., lossless PNG compression) rather than code changes.
**Action:** Use tools like `optipng` to reduce file sizes without quality loss. Handle filenames with spaces carefully in shell commands.
