# EduNexus 项目介绍主页

独立的静态展示站点。工作台由浏览器渲染预设界面与对话，不连接正式平台、不调用模型 API。

## 本地预览

在仓库目录运行：

```powershell
python -m http.server 4173
```

打开 http://localhost:4173/ 。不要直接双击 HTML：`file://` 下浏览器可能阻止模块脚本加载，导致工作台无法显示。

## GitHub Pages

在仓库的 **Settings → Pages → Build and deployment → Source** 选择 **GitHub Actions**。

推送到 `main` 后，`.github/workflows/pages.yml` 自动部署；也可在 Actions 页面手动运行 **Deploy EduNexus homepage**。

预期站点地址：https://bearcoder6.github.io/EduNexus-homepage/

## 页面资源

- `index.html`：项目介绍主页。
- `workspace-preview.html`：首屏工作台。
- `demo-workspace-preview.html`：四模式情景演示。
- `assets/`：工作台已打包脚本、样式、图像。

无需 npm、服务端或 API Key。部署时必须保留预览 HTML 与 `assets/` 的相对目录关系。
