# The Altered Circus — GitHub Pages

## 首次发布
1. 创建 GitHub 仓库（公开仓库通常最方便）。
2. 把本文件夹中的 index.html、stage-config.json、assets 文件夹和 .nojekyll 上传至仓库根目录。不要上传外层文件夹本身。
3. 仓库 Settings → Pages → Deploy from a branch → main / (root) → Save。
4. 等待 Pages 部署成功，打开提供的 HTTPS 网址。

观众入口：https://你的用户名.github.io/你的仓库名/
布置入口：https://你的用户名.github.io/你的仓库名/?setup=1
二维码应使用观众入口，不带 ?setup=1。

## 调整及发布
在布置入口点击右上角设置，或 STAGE SETUP；可切换现场相机和照片预览。调整位置、比例、灯光后点击“导出公共配置”。
把下载的文件命名为 stage-config.json，替换 GitHub 仓库根目录同名文件并提交。等待 Pages 部署完成后，观众刷新或重新打开网页即应用新配置。已经打开的页面不会实时自动更新。
导入 JSON 只修改你的本机草稿；导出也不会自动上传 GitHub。
“恢复已发布配置”恢复本次打开时下载的公共配置；要读取刚发布的新配置，刷新后再使用该按钮。
观众模式完全忽略本机草稿和旧版调试存储。布置模式草稿仅保存在本机浏览器。
?setup=1 用来显示布置界面，不是密码保护；访客修改只影响他们本机，不能写入网站。

## 发布前检查
- 在 iPhone Safari、Android Chrome 测试相机权限、画面方向、三个模型与介绍卡。
- 在实际夜间露台，从指定观看点调整。当前位置固定在屏幕上，尚未接入图像追踪，不会随真实露台自动定位。
- 测试修改 JSON 并重新发布后，观众入口在刷新后更新；测试拒绝相机权限后的提示与照片预览。
- 配置读取失败时使用内置默认值，布置界面显示原因。file:// 本地预览无法读取公共 JSON，使用内置默认值；请在 Pages HTTPS 地址验证配置。

## 文件与限制
模型已嵌入 index.html，因此不用上传 .blend、独立 GLB 或工作脚本。Three.js 与 GLTFLoader 来自 jsDelivr，需要网络。相机需要 HTTPS。站点是静态网站，上传 JSON 后发布配置，无后台、无自动保存到 GitHub、无实时同步。
