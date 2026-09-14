# 亚星形态 · 第三阶段跟踪

这是“亚星形态”选股项目第三阶段的静态观察池看板。

## GitHub Pages 发布

仓库内置 GitHub Actions 工作流。推送到 `main` 分支后，工作流会把 `dist/` 发布到 GitHub Pages。

首次发布时，在仓库的 **Settings → Pages → Build and deployment** 中将 **Source** 设为 **GitHub Actions**。

## 本地文件

- `dist/index.html`：看板页面
- `dist/tracker.json`：每日跟踪数据
- `dist/klines.json`：观察候选近120个交易日的前复权日K数据
- `dist/update-status.json`：盘后流水线校验状态与生成时间

页面使用相对路径读取 `tracker.json` 和 `klines.json`，点击股票后可查看30/60/120日K线，可同时部署在 GitHub Pages 的项目子路径下。

