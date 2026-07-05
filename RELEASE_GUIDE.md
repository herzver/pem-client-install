# GitHub / Gitee Release 发布指南

本文用于发布 `pem-client-install` 仓库的新版本安装包。

## 版本命名

建议统一使用：

```text
v3.5.4
```

Release 标题：

```text
和智慧明镜 PEM Windows 客户端 v3.5.4
```

安装包文件名：

```text
herzver_pem_setup_3.5.4.exe
```

## 发布前检查

1. 确认安装包能正常安装、启动、登录。
2. 确认安装包版本号与产品版本一致。
3. 更新 `README.md` 中的当前安装包名称。
4. 更新百度网盘文件，确认分享链接和提取码可用。
5. 同步推送到 GitHub 和 Gitee。

## GitHub Release 操作

网页方式：

1. 打开 GitHub 仓库：`https://github.com/DavaLin/pem-client-install`
2. 进入右侧或顶部的 `Releases`。
3. 点击 `Draft a new release`。
4. `Choose a tag` 填写：`v3.5.4`。
5. Release title 填写：`和智慧明镜 PEM Windows 客户端 v3.5.4`。
6. 上传安装包：`herzver_pem_setup_3.5.4.exe`。
7. 填写 Release notes。
8. 点击 `Publish release`。

Release notes 模板：

```markdown
## 和智慧明镜 PEM Windows 客户端 v3.5.4

本版本提供明镜 PEM 项目经营核算系统 Windows 客户端安装包。

### 下载

- 百度网盘： https://pan.baidu.com/s/10i81SKAYz232k8w4tqD9Xw?pwd=hpem
- GitHub Release：见本页面附件
- Gitee 镜像： https://gitee.com/dava_lin/pem-client-install

### 使用说明

- 支持 Windows 10 / Windows 11。
- 客户端需要联网使用。
- Windows 客户端和网页端数据、账号、权益完全打通。
- 可长期免费使用。

### 适用团队

适合广告公司、活动执行、策划设计、物料制作、影视拍摄、展陈装饰等项目制团队，用于核算项目成本、外协、回款和真实利润。
```

命令行方式（可选）：

```powershell
gh release create v3.5.4 "herzver_pem_setup_3.5.4.exe" `
  --repo DavaLin/pem-client-install `
  --title "和智慧明镜 PEM Windows 客户端 v3.5.4" `
  --notes-file release-notes-v3.5.4.md
```

使用命令行方式前，需要安装并登录 GitHub CLI：`gh auth login`。

## Gitee Release 操作

网页方式：

1. 打开 Gitee 仓库：`https://gitee.com/dava_lin/pem-client-install`
2. 进入 `发行版` / `Releases`。
3. 点击 `创建发行版`。
4. 标签名填写：`v3.5.4`。
5. 发行版标题填写：`和智慧明镜 PEM Windows 客户端 v3.5.4`。
6. 上传安装包：`herzver_pem_setup_3.5.4.exe`。
7. 填写发行说明，可复用 GitHub Release notes。
8. 发布发行版。

如果 Gitee 页面提示必须先有 tag，可以先在本地创建并推送 tag：

```powershell
git tag v3.5.4
git push origin v3.5.4
git push gitee v3.5.4
```

## 每次发版后的同步事项

1. README 当前安装包名称。
2. GitHub Release。
3. Gitee Release。
4. 百度网盘文件。
5. 官网下载落地页里的版本号和下载说明。
6. 如有二维码、短链接或销售资料，也同步更新。
