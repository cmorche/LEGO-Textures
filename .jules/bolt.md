## 2025-01-05 - Found Unoptimized PNGs
**Learning:** The repository contains several large PNG files (e.g., `Ninjago/Slithra/Slithra Head.png` ~516K) that are not optimized. `optipng` can significantly reduce their size without losing quality.
**Action:** Run `optipng -o7` on large assets to improve download speeds and reduce repository size.
## 2025-12-31 - [Asset Optimization]
**Learning:** This repository consists entirely of static assets with no build system. Performance gains come exclusively from optimizing these assets (e.g., lossless PNG compression) rather than code changes.
**Action:** Use tools like `optipng` to reduce file sizes without quality loss. Handle filenames with spaces carefully in shell commands.

## 2025-01-27 - [Zopflipng Timeouts]
**Learning:** `zopflipng` is highly effective but slow. Running it on a batch of 10 large files sequentially in a single script caused a timeout (>400s).
**Action:** Process large files individually or in very small batches (2-3 files) when using `zopflipng` to ensure completion and avoid timeouts.
