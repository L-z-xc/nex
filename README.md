# nex

本仓库包含可直接安装到 DeepSeek Harness (DSH) 的 dsh-purge-community 插件包。

## 文件
- $(dsh-purge-community-1.6.84.tgz.Name)：npm 打包的可安装插件包（推荐）
- dsh-purge-community/：插件源码目录（含 package.json、cordis.patch.yml、lib/、client.js 等）

## 在其他电脑的 DSH 中安装
1. 下载本仓库中的 $(dsh-purge-community-1.6.84.tgz.Name) 到本机。
2. 在 DSH 插件管理/CLI 中安装该包（任选其一）：
   - 若使用 DSH CLI：dsh plugin add "C:\path\to\dsh-purge-community-1.6.84.tgz"
   - 或在 DSH「插件/扩展」界面选择从本地文件/包安装，指向该 .tgz。
3. 安装后按需重启 DSH 使插件生效。

> 版本：dsh-purge-community 1.6.84（从本机 dsh-purge-1.6.84 源打包）
