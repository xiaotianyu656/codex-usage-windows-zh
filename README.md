# Codex 额度监控（中文版）

基于 [guberm/Codex-Usage-Windows](https://github.com/guberm/Codex-Usage-Windows) v0.1.3 的中文改版，感谢原作者 Michael Guber。

Windows 10/11 x64 桌面悬浮工具，显示 Codex 额度、重置时间和可用重置次数。界面、菜单及提示已汉化；收起详情后悬浮条仍留在桌面，可通过“隐藏到托盘”隐藏。

## 构建

安装 .NET 10 SDK 后，在仓库目录运行：

```powershell
dotnet publish src/CodexUsage.csproj -c Release -r win-x64 -o publish
```

生成的单文件 EXE 自带运行环境。登录使用 OpenAI 设备授权，凭据由 Windows 当前用户加密保存在本机。此项目为非官方工具，使用第三方客户端涉及账户令牌；请自行评估风险。重置按钮会消耗可用重置次数，并有确认提示。

## 许可与来源

原项目 Copyright (c) 2026 Michael Guber，基于 MIT 许可发布。原版权与许可见 [LICENSE](LICENSE)。本项目为中文翻译及收起行为调整。
