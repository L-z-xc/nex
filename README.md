# nex

本仓库包含可直接安装到 DeepSeek Harness (DSH) 的 `dsh-purge-community` 插件（npm 包形式）。

## 内容
- `dsh-purge-community/`：npm 包源码目录（含 `package.json`、`cordis.patch.yml`、`lib/`、`client.js` 等），可直接 `npm pack` / `npm publish`
- `dsh-purge-community-1.6.84.tgz`：已打包的 npm 包（tgz），可直接用于安装

## 作为 npm 包打包
在包目录内执行：
```bash
cd dsh-purge-community
npm pack
```
会在当前目录生成 `dsh-purge-community-1.6.84.tgz`（标准 npm 包格式，可用于安装或发布）。

## 在其他电脑的 DSH 中安装
1. 获取 `dsh-purge-community-1.6.84.tgz`（从本仓库下载，或自行 `npm pack` 生成）。
2. 任选其一安装：
   - DSH CLI：`dsh plugin add "C:\path\to\dsh-purge-community-1.6.84.tgz"`
   - 或在 DSH「插件/扩展」管理中选择从本地文件/包安装，指向该 `.tgz`。
3. 安装后按需重启 DSH 使插件生效。

若该包已发布到 npm registry，也可按 DSH 的 npm 安装方式安装对应包名/版本（例如 `dsh-purge-community@1.6.84`）。

## 发布到 npm（可选）
```bash
cd dsh-purge-community
npm login
npm publish --access public
```
> 发布前请确认你拥有 npm 上该包名的发布权限，并按需调整 `package.json` 中的 `name`/`version`。

> 版本：`dsh-purge-community@1.6.84`（基于本机 `dsh-purge-1.6.84` 源整理）
