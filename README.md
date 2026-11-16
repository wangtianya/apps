# Apps

官方下载入口：https://apps.tianya.pub

本仓库只保存公开安装包、校验文件、更新说明和静态下载站。应用源码和内部发行登记位于私有仓库。

测试版和正式版独立；安装包在 Releases 按应用和环境保存，完整成功历史保留。网页不调用 GitHub API。

维护应用资料：`data/apps.json`。发行数据由本机发布器写入 `data/<app>/<environment>/`，不要手工覆盖版本。下载站使用 Wrangler 直接上传到 Cloudflare Pages 项目 `apps-downloads`；GitHub Pages 和 GitHub Actions 均不参与部署。

本地预览：`python3 -m http.server 8080`。没有安装包的应用显示“尚未发布”。
