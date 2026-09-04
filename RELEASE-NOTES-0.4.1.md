# TAIL 0.4.1 Preview

发布日期：2026-09-04

这是 TAIL 第一个可下载的 Windows 早期预览。它用于展示当前桌面工作区、右侧工具区、TAIL 助手、个性化、只读研究入口和安全状态表达。

## 下载选择

- `TAIL-V0.4.1-Preview-Setup-x64.exe`：Windows x64 安装版；
- `TAIL-V0.4.1-Preview-Portable-x64.exe`：Windows x64 便携版；
- `SHA256SUMS.txt`：两个文件的 SHA-256 校验值。

## 重要提示

- 当前 EXE **未进行 Authenticode 代码签名**，Windows 可能显示未知发布者或 SmartScreen 提示；
- 只从 `Tailovo/tail-trading-workspace` 的 GitHub Release 下载；
- 本版本是早期开发预览，不是最终产品；
- 本版本不是自动实盘产品，不连接钱包，也不提供签名、广播、真实下单、自动卖出或清仓；
- 合成回测和 Fixture 只用于界面/数据链路验证，不证明收益。

## 本次主要变化

- 新工作区布局、分组导航和多模式右侧工具区；
- 行情与 K 线空状态、内置研究浏览器、诊断与证据入口；
- TAIL 助手拖动与状态交互；
- 主题、背景、透明度、工作区颜色与减少动画；
- 合成回测、持仓 Fixture、断连状态场景；
- 独立只读 Showcase API 与无远程请求市场实现；
- 私有研究任务入口锁定并从安装包物理排除。

## 发布前验证

- 2049 个测试通过、5 个跳过；
- Lint、TypeScript、服务端、Web 与桌面构建通过；
- 最终安装包烟雾测试退出码 0；
- ASAR 中仅 9 个应用文件；
- 未检出源码映射、任务脚本、生产启动器、生产 Canary、已知钱包、私人路径或疑似凭据；
- 两个 EXE 在构建机当前 Microsoft Defender 定义下均未发现威胁。

Microsoft Defender 结果不是第三方安全认证。请自行核对 SHA-256 并使用终端防护软件。

## SHA-256

```text
2F579E10EEFEA866D38C23BC37F39E47FC1401EC4E79B10CD5C9D26B32DEC7F0  TAIL-V0.4.1-Preview-Portable-x64.exe
E5E346F0EFF166ED820E162770982167B5079CAEFD0EC909A27EB751C7837BBB  TAIL-V0.4.1-Preview-Setup-x64.exe
```

## 已知限制

- 未签名；
- 公开包默认离线/断连；
- 私有研究任务和生产执行不包含；
- 当前没有开源许可证；
- 不承诺收益、可用性或容量；
- UI、交互和数据接入仍会继续变化。
