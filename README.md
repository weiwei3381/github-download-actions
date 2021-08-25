# github-download-actions

使用 GitHub Actions 下载外网文件。

## 原理

使用 GitHub Actions 的服务器，从外网下载文件。将需要下载的视频添加到 urlList.txt 文件中，每次 push 的时候，github action 读取 urlList.txt 列表，并下载列表中的所有文件。

## 使用

- 点右上角 **Fork** 按钮复制本 GitHub 仓库
- 在自己的项目中，点上方 **Actions** 选项卡进入项目 GitHub Actions 页面, 点击绿色按钮 “**I understand my workflows, go ahead and enable them**” 开启自动提交功能
- 编辑 [urlList.txt](./urlList.txt) 文件，将下载的url添加到列表中
- 等待 github action 执行成功，视频会出现在 [downloads](./downloads/) 目录
