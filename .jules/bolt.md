## 2025-01-05 - Found Unoptimized PNGs
**Learning:** The repository contains several large PNG files (e.g., `Ninjago/Slithra/Slithra Head.png` ~516K) that are not optimized. `optipng` can significantly reduce their size without losing quality.
**Action:** Run `optipng -o7` on large assets to improve download speeds and reduce repository size.
## 2025-12-31 - [Asset Optimization]
**Learning:** This repository consists entirely of static assets with no build system. Performance gains come exclusively from optimizing these assets (e.g., lossless PNG compression) rather than code changes.
**Action:** Use tools like `optipng` to reduce file sizes without quality loss. Handle filenames with spaces carefully in shell commands.

## 2025-01-05 - Batch Optimization Timeout
**Learning:** Running `optipng -o7` on a batch of files caused a timeout due to high CPU usage per file. Lowering to `optipng -o2` was significantly faster and still yielded ~10-30% file size reduction for unoptimized assets.
**Action:** Use `-o2` for batch optimization or process files in smaller chunks when using higher compression levels.
