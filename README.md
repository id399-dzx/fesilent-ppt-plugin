# fesilent-ppt-插件

插件产品名：**Fesilent-sci（费思量）**。

用于 Windows 桌面版 PowerPoint 的科研绘图与排版插件。安装后在 PowerPoint 顶部显示 **Fesilent-sci** 选项卡。

[下载最新版安装包](https://github.com/id399-dzx/fesilent-ppt-plugin/releases/latest)

## 功能

| 功能 | 用途 |
| --- | --- |
| 参数化圆环 | 创建可编辑的多层圆环，设置分段、圆角、箭头、颜色和渐变，实时调整图形 |
| 分类模板图库 | 保存选中图形为模板，预览并插入可编辑模板 |
| 图形导出 | 导出 PNG、TIFF、BMP、JPEG、SVG、EMF；位图可设置 DPI，按可见内容裁边 |
| 纹理上色 | 显微图片伪彩色分区，手动修正区域，导出图片或插入幻灯片 |
| 科研组图 | 自动排列图片、批量添加标签与图题、框选局部并创建放大图 |

2026-10-05 更新了科研组图功能。局部放大保留原图，使用 PowerPoint 原生裁剪副本；标签和图题使用可编辑文本框。详细说明见 [本次发布说明](release-notes.md)。

## 安装

1. 在 Releases 下载 `Fesilent-sci-0.2.1-Windows-Setup.zip` 并解压。
2. 保存演示文稿，完全关闭 PowerPoint。
3. 运行 `Fesilent-sci-Setup.exe`，点击“安装 / 更新”。
4. 重新打开 PowerPoint，查看顶部 **Fesilent-sci** 选项卡。

需要 Windows 桌面版 PowerPoint 和 .NET Framework 4.8；按当前 Windows 用户安装，无需管理员权限，兼容 32 位和 64 位 PowerPoint。安装程序尚未代码签名。安装包提供文件 SHA-256 校验清单，Release 另附整个 ZIP 的校验值。

## 使用与限制

科研组图：先选中图片，打开对应功能，点击“读取当前选择”，调整参数后应用。首次支持每次 1–100 张独立、未旋转、未翻转图片；局部放大一次选择一张。放大图、区域框和连接线分别编辑，移动后不自动联动。

纹理分区用于展示用伪彩色初稿，不能替代真实晶粒或材料分类；低分辨率图片也不会因提高导出 DPI 恢复细节。

安装包内的 `install-readme.txt` 包含更新、卸载和故障诊断步骤。诊断报告含本机用户名和路径，请自行检查后再决定是否分享。

本仓库提供插件安装包及使用说明。
