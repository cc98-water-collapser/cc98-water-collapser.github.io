# CC98 水帖折叠器 · GitHub Pages 项目页

这是一个可直接放进 GitHub 仓库根目录的静态网页项目，包含：

- index.html：介绍页与安装说明。
- assets/：你提供的四张弹窗、设置及折叠前后效果图。
- downloads/CC98水帖折叠器_v1.3.0.zip：你提供的 dist1.3.0.zip 原样副本，仅改外层文件名。
- .nojekyll：让 GitHub Pages 按普通静态文件方式发布。

## 发布到 GitHub Pages

1. 登录 GitHub，创建一个公开仓库，例如 cc98-water-collapser。
2. 在仓库首页选择 **Add file → Upload files**，把本目录里的 index.html、README.md、.nojekyll、assets 文件夹和 downloads 文件夹上传到仓库根目录。确认仓库首页就能看到 index.html、assets/ 和 downloads/。
3. 打开仓库 **Settings → Pages**。在 **Build and deployment** 中选择 **Deploy from a branch**，分支选 main，目录选 /(root)，保存。
4. 等 Pages 部署完成后，访问 GitHub 显示的网页地址。页面的下载按钮会下载 downloads/ 下的 ZIP。
5. （推荐）再打开仓库 **Releases → Create a new release**，标签设为 v1.3.0，上传同一个 ZIP 作为 Release 附件。发布后，页面会在 GitHub Pages 环境里显示通往 /releases/latest 的按钮。

后续更新时，替换页面和 ZIP，并给新版本创建新的 Release 标签；不要复用旧标签覆盖旧附件。

## 下载包信息

网页附带的 ZIP 是所提供压缩包的原样副本。压缩包内部目录为 dist1.3.0/，manifest.json 位于该目录内；解压后选择 dist1.3.0 文件夹加载即可。

- 文件大小：32,625 字节（约 32.6 KB）
- SHA-256：DB8189F1990975831EC3D3C42D4C3515526EEF25432C8D779835F80422BD23F9

原发帖文案写着另一个 SHA-256（69eed7...）和 30.7 KB；它们与本次收到的 ZIP 不一致。发布前请把帖子文案中的文件大小和校验值更新为上面实测结果。

## 图片说明

网页将四张图片保存在 assets/ 中，部署后直接从仓库加载，不依赖原文里的外链图床。两张帖子折叠效果图沿用原文说明，是虚构内容演示，并非真实 CC98 帖子截图。

本次收到的 ZIP 只有扩展的打包产物（dist），没有扩展源代码工程或构建脚本。因此这个目录提供网页源码和可下载的扩展包；若要在 GitHub 同时公开扩展源代码，还需要补充原始源码仓库内容。

## 手动安装扩展

1. 下载 ZIP 并解压。
2. Chrome 打开 chrome://extensions/，Edge 打开 edge://extensions/，启用开发者模式。
3. 选择“加载已解压的扩展程序”，选解压出来的 dist1.3.0 文件夹（该目录下直接有 manifest.json）。
4. 打开 CC98 帖子页并刷新。
