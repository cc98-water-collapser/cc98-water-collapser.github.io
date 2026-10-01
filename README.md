# CC98 水帖折叠器 · GitHub Pages 项目页

这是一个可直接放进 GitHub 仓库根目录的静态网页项目，包含：

- index.html：介绍页与安装说明。
- downloads/CC98水帖折叠器_v1.3.0.zip：从你提供的 dist1.3.0.zip 原样复制并改成便于发布的文件名。
- .nojekyll：让 GitHub Pages 按普通静态文件方式发布。

## 发布到 GitHub Pages

1. 登录 GitHub，创建一个公开仓库，例如 cc98-water-collapser。
2. 在仓库首页选择 **Add file → Upload files**，把本目录里的 index.html、README.md、.nojekyll 和 downloads 文件夹中的 ZIP 上传到仓库根目录。确认仓库首页就能看到 index.html 和 downloads/。
3. 打开仓库 **Settings → Pages**。在 **Build and deployment** 中选择 **Deploy from a branch**，分支选 main，目录选 /(root)，保存。
4. 等 Pages 部署完成后，访问 GitHub 显示的网页地址。页面的下载按钮会下载 downloads/ 下的 ZIP。
5. （推荐）再打开仓库 **Releases → Create a new release**，标签设为 v1.3.0，上传同一个 ZIP 作为 Release 附件。发布后，页面会在 GitHub Pages 环境里显示通往 /releases/latest 的按钮。

后续更新时，替换页面和 ZIP，并给新版本创建新的 Release 标签；不要复用旧标签覆盖旧附件。

## 下载包信息

网页附带的 ZIP 是所提供压缩包的原样副本，仅改了外层文件名。压缩包内部目录为 dist1.3.0/，manifest.json 位于该目录内；解压后选择 dist1.3.0 文件夹加载即可。

- 文件大小：32,625 字节（约 32.6 KB）
- SHA-256：DB8189F1990975831EC3D3C42D4C3515526EEF25432C8D779835F80422BD23F9

提供的发帖文案写着另一个 SHA-256（69eed7...）和 30.7 KB；它们与本次收到的 ZIP 不一致。发布前请把帖子文案中的文件大小和校验值更新为上面实测结果。

## 当前素材说明

效果图、弹窗和设置页图片使用文案里的 file.cc98.org 外链。如果外链失效，可将图片保存到仓库中的 assets/ 后，替换 index.html 里的对应图片地址。两张帖子效果图按原文说明属于虚构内容演示，并非真实 CC98 帖子截图。

本次收到的 ZIP 只有扩展的打包产物（dist），没有扩展源代码工程或构建脚本。因此这个目录提供网页源码和可下载的扩展包；若要在 GitHub 同时公开扩展源代码，还需要补充原始源码仓库内容。

## 手动安装扩展

1. 下载 ZIP 并解压。
2. Chrome 打开 chrome://extensions/，Edge 打开 edge://extensions/，启用开发者模式。
3. 选择“加载已解压的扩展程序”，选解压出来的 dist1.3.0 文件夹（该目录下直接有 manifest.json）。
4. 打开 CC98 帖子页并刷新。
