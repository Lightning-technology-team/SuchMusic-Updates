# SuchMusic-Updates

**SuchMusic 概念版**的安装包与更新清单仓库。

- `public/latest.apk`：最新安装包（始终指向当前内测版）
- `public/update.json`：App 内置的「检查更新」读取的清单
- `public/index.html`：下载落地页

本仓库由 [Cloudflare Pages](https://pages.cloudflare.com/) 部署，通过自定义域名
`dl.lightning-team.de5.net` 对外提供下载（国内访问速度优于 GitHub Releases）。

> 部署：推送 `main` 分支后 Cloudflare Pages 自动构建（构建命令 `exit 0`，输出目录 `public`）。
