# CC98 水帖折叠器 · GitHub Pages

这是插件产品官网落地页，页面按“产品效果 → 功能 → 使用流程 → 优势 → 下载”展开。页面截图及弹窗、设置图保存在 assets/ 中，不依赖外链图床。

## 发布到 GitHub Pages

1. 在 GitHub 创建公开仓库，例如 cc98-water-collapser。
2. 把本项目中的 index.html、README.md、assets/ 和 downloads/ 上传到仓库根目录。
3. 打开 **Settings → Pages**，选择 **Deploy from a branch**，分支选 main，目录选 /(root)，保存。
4. Pages 部署完成后，访问 GitHub 提供的网址。页面下载按钮会获取 downloads/ 中的扩展包。
5. 推荐另建 GitHub Release，标签使用 v1.3.0 并附上同一个 ZIP；页面会显示该仓库的 latest Release 链接。

## 页面文件

- index.html：响应式产品落地页源码。
- assets/：弹窗、设置页、折叠前后效果图及 2880 × 6840 高清页面设计稿。
- downloads/CC98水帖折叠器_v1.3.0.zip：提供的扩展压缩包原样副本，仅改外层文件名。

## 下载包校验信息

- 文件大小：32,625 字节（约 32.6 KB）
- SHA-256：DB8189F1990975831EC3D3C42D4C3515526EEF25432C8D779835F80422BD23F9

原发帖文案里的大小和 SHA-256 与实际附件不符，发布前请使用上面的实测值更新。

ZIP 内部目录为 dist1.3.0/，其中直接包含 manifest.json；解压后加载 dist1.3.0 文件夹即可。

## 安装方式

1. 下载 ZIP 并解压。
2. Chrome 打开 chrome://extensions/，Edge 打开 edge://extensions/，启用开发者模式。
3. 选择“加载已解压的扩展程序”，选解压出的 dist1.3.0 文件夹。
4. 打开 CC98 帖子页并刷新。

本次附件只有扩展打包产物，不包含扩展原始源码工程或构建脚本。
