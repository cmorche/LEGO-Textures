## 2025-01-05 - Found Unoptimized PNGs
**Learning:** The repository contains several large PNG files (e.g., `Ninjago/Slithra/Slithra Head.png` ~516K) that are not optimized. `optipng` can significantly reduce their size without losing quality.
**Action:** Run `optipng -o7` on large assets to improve download speeds and reduce repository size.
## 2025-12-31 - [Asset Optimization]
**Learning:** This repository consists entirely of static assets with no build system. Performance gains come exclusively from optimizing these assets (e.g., lossless PNG compression) rather than code changes.
**Action:** Use tools like `optipng` to reduce file sizes without quality loss. Handle filenames with spaces carefully in shell commands.
## 2026-01-28 - [Monster Fighters Optimization]
**Learning:** Significant size reductions (~18-30%) were achieved in `Monster Fighters` assets using `zopflipng`, even on files `optipng` might consider optimized. `zopflipng` is slower but yields better compression.
**Action:** Prioritize `zopflipng` for asset optimization where build time allows. Focus on deeper directories like `Monster Fighters` which may have been skipped in previous passes.
