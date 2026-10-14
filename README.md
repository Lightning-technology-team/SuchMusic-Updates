# SuchMusic-Updates

**SuchMusic 概念版**的更新清单与下载落地页（由 Cloudflare Pages 自本仓库构建部署）。

- `public/update.json`：App 内置「检查更新」读取的清单（含 Cloudflare 下载直链）
- `public/index.html`：下载落地页

## 为什么安装包不放在这里

Cloudflare Pages 对**单个文件有 25 MiB 上限**，而 APK 约 46 MiB，无法直接托管。
因此安装包由 Cloudflare **Worker**（`dl.lightning-team.de5.net/latest.apk`）从
GitHub Releases 边缘代理并缓存，下载仍走 Cloudflare 节点（国内更快）。
