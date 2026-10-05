Fesilent-sci（费思量）0.2.1 · Windows PowerPoint 安装包

系统要求
• Windows 桌面版 PowerPoint（Microsoft 365 或支持 COM 加载项的桌面版本）
• .NET Framework 4.8 或更高版本
• 当前 Windows 用户具有写入自己的 AppData 和注册表的权限

安装
1. 解压本压缩包，双击 Fesilent-sci-Setup.exe。
2. 保存演示文稿并完全关闭 PowerPoint，然后点击“安装 / 更新”。
3. 重新打开 PowerPoint。顶部出现“Fesilent-sci”选项卡；“模板图库”右侧的“导出图片”可导出选中图形。

2026-10-05 更新：科研组图
“Fesilent-sci → 科研组图”提供自动排列、批量标签、批量图题和局部放大。先选中图片，打开对应功能，点击“读取当前选择”，设置参数后应用。
自动排列保持图片比例；标签和图题使用可编辑文本框，重复应用会更新已有内容。局部放大保留原图，可在预览或大图窗口拖动框选，使用 PowerPoint 原生裁剪副本生成放大图，并可添加区域框与连接线。
首版处理独立、未旋转、未翻转图片，局部放大一次选择一张；区域框、放大图和连接线分别编辑，移动后不自动联动。各项操作支持 PowerPoint 撤销。详见 release-notes.md。

导出图片支持 PNG、TIFF、BMP、JPEG 和 SVG、EMF。位图可选择 DPI，按实际可见内容裁边；PNG/TIFF 保留透明，BMP/JPEG 为白底。多选图形会合成为一张图片。SVG/EMF 沿用 PowerPoint 原生矢量边界，不适用 DPI。

更新前请确认任务管理器中没有 POWERPNT.EXE 进程。只关闭窗口而后台进程未退出时，PowerPoint 仍可能加载旧版插件；安装程序也会拒绝在 PowerPoint 运行时更新。

安装按当前 Windows 用户进行，不需要管理员权限。兼容 32 位和 64 位 PowerPoint。
如电脑上已经手工安装过旧版圆环工具，安装程序会停止并提示先卸载旧版，以保护原有注册。
插件的模板、参数方案和自定义颜色保存在当前用户的 AppData 中；卸载程序不会删除这些数据。

卸载
在 Windows“已安装的应用”中选择“Fesilent-sci（费思量）”并卸载，或再次运行安装程序，点击“卸载插件”。操作前请关闭 PowerPoint。

说明
这是未使用代码签名证书签名的安装程序。Windows 首次运行时可能显示发布者未知提示。
SHA256.txt 列出了安装程序与说明文件的校验值。安装程序还会验证内置 DLL 的 SHA-256，校验失败时拒绝安装。

故障诊断
如果安装程序显示成功，但 PowerPoint 中没有 Fesilent-sci，保持 PowerPoint 打开，在当前用户账户下双击 Run-Diagnosis.cmd。桌面会生成 Fesilent-sci-diagnostic.txt。请先查看其中的 Windows 用户名、加载项注册、Office 策略和 PowerPoint 发现情况，再决定是否分享报告；报告含当前用户名和本机安装路径。
