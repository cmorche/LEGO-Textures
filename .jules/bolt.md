# Bolt's Journal

## 2024-05-22 - [Optimizing Asset-Only Repositories]
**Learning:** In repositories that consist solely of static assets (like images) with no application code, "performance optimization" means minimizing file sizes without quality loss. This directly improves download speeds and bandwidth usage for consumers of the assets.
**Action:** When facing asset-only repos, prioritize lossless compression of the largest files and consider adding automation (like GitHub Actions) to prevent future regression, although tooling constraints might limit immediate implementation of automation.
