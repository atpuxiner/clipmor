# Clipmor 使用说明

Clipmor 是一款轻量极简、低资源占用的 Windows 剪贴板增强工具。

剪贴历史支持保存文本与图片、新建、删除、关键词搜索、置顶，记录为系统复制原始数据，不提供编辑；内置简洁的待办功能，支持新建、编辑、删除、关键词搜索、置顶显示。
所有数据全部保存在本地 SQLite 数据库，不上传网络、不收集隐私信息，完全离线可用。

[English](README.en.md) | [简体中文](README.md)

## 下载

### 微软商店（推荐）

在 Microsoft Store 中搜索 `Clipmor` 即可安装：

[Clipmor Microsoft Store](https://apps.microsoft.com/detail/9p5qx0dxvlfk)

### GitHub Releases

打开 [GitHub Releases 发布页](https://github.com/atpuxiner/clipmor/releases)，选择最新版本，根据需求下载对应版本：

- **便携版** `Clipmor-portable-x64-vX.X.X.X.zip`：免安装，解压即用。
- **安装版** `Clipmor-setup-x64-vX.X.X.X.exe`：一键安装，可选择创建桌面快捷方式。

## 开始使用

### 便携版

1. 下载并解压最新的便携包（如 `Clipmor-portable-x64-vX.X.X.X.zip`），得到一个 `clipmor.exe` 文件。
2. 双击运行即可，无需安装。
3. 正常复制内容，然后按 `Ctrl+Q` 打开历史窗口。

### 安装版

1. 下载并运行最新的安装程序（如 `Clipmor-setup-x64-vX.X.X.X.exe`），按提示完成安装。
2. 从开始菜单或桌面快捷方式启动 Clipmor。
3. 正常复制内容，然后按 `Ctrl+Q` 打开历史窗口。

## 数据存储位置

- **安装版**：`%LOCALAPPDATA%\Clipmor`
- **便携版**：exe 所在目录或 `%LOCALAPPDATA%\Clipmor`

数据文件包括：

```text
clipmor.db       # 文本历史记录
clipmor.imgs/    # 图片历史记录
```

## 核心功能

- 剪贴历史：保存文本、图片记录，新建、删除、搜索、置顶常用内容
- 快速检索：关键词搜索，快速定位历史剪贴记录
- 置顶显示：高频内容固定顶部，随时取用
- 待办清单：内置简单待办，可新建、编辑、删除、搜索、置顶
- 轻量后台：体积小巧，托盘静默运行，性能开销低
- 可控自启：开机自启默认关闭，由用户手动开启

## 备份与迁移

- 数据库已加密，`clipmor.db` 不能直接拷到另一台电脑或另一 Windows 用户下使用。
- 跨机迁移：在原电脑点击“导出”生成 CSV，再到新电脑点击“导入”即可；图片记录需连同 `clipmor.imgs/` 中对应图片文件一起拷贝。

## 常见问题

- 程序打不开：请确认 `clipmor.exe` 没有被杀毒软件拦截。
- 看不到历史：先复制一些内容，再按 `Ctrl+Q` 打开历史窗口即可。
- 历史不见了：先确认数据存放位置（详见上文“数据存储位置”），再检查对应的 `clipmor.db` 和 `clipmor.imgs/` 是否仍在且未被删除。
- 兼容的系统：支持 Windows 10 / 11。

## 开源许可

本项目基于 MIT 许可证（MIT License）发布，详见 [LICENSE](LICENSE)。
