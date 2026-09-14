# 亚星形态 · 第三阶段跟踪

这是“亚星形态”选股项目第三阶段的静态观察池看板。

## GitHub Pages 发布

仓库内置 GitHub Actions 工作流。推送到 `main` 分支后，工作流会把 `dist/` 发布到 GitHub Pages。

首次发布时，在仓库的 **Settings → Pages → Build and deployment** 中将 **Source** 设为 **GitHub Actions**。

## 本地文件

- `dist/index.html`：看板页面
- `dist/tracker.json`：每日跟踪数据

页面使用相对路径读取 `tracker.json`，可同时部署在 GitHub Pages 的项目子路径下。
