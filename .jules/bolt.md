## 2025-01-05 - Found Unoptimized PNGs
**Learning:** The repository contains several large PNG files (e.g., `Ninjago/Slithra/Slithra Head.png` ~516K) that are not optimized. `optipng` can significantly reduce their size without losing quality.
**Action:** Run `optipng -o7` on large assets to improve download speeds and reduce repository size.
## 2025-12-31 - [Asset Optimization]
**Learning:** This repository consists entirely of static assets with no build system. Performance gains come exclusively from optimizing these assets (e.g., lossless PNG compression) rather than code changes.
**Action:** Use tools like `optipng` to reduce file sizes without quality loss. Handle filenames with spaces carefully in shell commands.

## 2025-01-25 - [Asset Optimization Wins]
**Learning:** Found significant reductions in 'older' assets (e.g., Cave Girl Torso reduced by ~78KB/28%), confirming the README's note about older textures being less refined.
**Action:** Prioritize optimization of assets in older series/folders as they likely yield better compression ratios.
