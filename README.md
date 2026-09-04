# TAIL

> 一个把观察、研究、风险与状态证据放在一起的桌面交易工作台。

TAIL 仍处于早期开发阶段。当前公开的是一个 Windows x64 可运行预览，用来展示桌面工作区、状态边界、研究入口和本地只读交互；它不是自动实盘产品，也不代表最终界面。

![TAIL 0.4.1 运行总览](assets/screenshots/tail-overview-v0.4.1.png)

## 下载 Windows 预览

| 版本 | 适合场景 | 下载 |
| --- | --- | --- |
| 安装版 | 正常安装到当前 Windows 用户 | [TAIL-V0.4.1-Preview-Setup-x64.exe](https://github.com/Tailovo/tail-trading-workspace/releases/download/v0.4.1-preview/TAIL-V0.4.1-Preview-Setup-x64.exe) |
| 便携版 | 不安装，直接运行单个 EXE | [TAIL-V0.4.1-Preview-Portable-x64.exe](https://github.com/Tailovo/tail-trading-workspace/releases/download/v0.4.1-preview/TAIL-V0.4.1-Preview-Portable-x64.exe) |

本预览包**尚未进行商业代码签名**，Windows SmartScreen 可能提示未知发布者。只从本仓库的 Release 页面下载，并使用 [SHA256SUMS.txt](https://github.com/Tailovo/tail-trading-workspace/releases/download/v0.4.1-preview/SHA256SUMS.txt) 校验文件。详细限制见 [0.4.1 发布说明](RELEASE-NOTES-0.4.1.md)。

## 这次可以实际体验什么

- 重新整理后的无残边桌面工作区与分组导航；
- 运行总览、实时信号、交易执行、持仓与退出、机会观察、策略、数据分析、研究、系统和诊断等入口；
- 可切换的右侧工具区：运行状态、行情与 K 线、内置浏览器、诊断与证据；
- 本地合成样本回测与明确标注的只读 Fixture（固定测试样本）；
- 主题、工作区颜色、背景、透明度、减少动画等个性化设置；
- 可拖动的 TAIL 助手及本地状态提示；
- 离线、断连、未知和未证明状态的真实呈现。

[查看完整界面导览](PRODUCT-TOUR.md)

## 为什么很多地方显示“未连接”或“暂不可用”

公开预览故意不携带生产账户、钱包、私钥、Token、研究任务脚本或真实执行配置。没有可核实数据时，界面不会用历史值、随机值或伪造行情补位。

因此你看到的“未连接”“暂不可用”“未授权”和“已锁定”不是演示故障，而是产品的安全边界。

## 公开包不具备什么

- 不连接钱包，不读取真实余额；
- 不包含签名、广播、真实下单或自动卖出能力；
- 不包含私有研究任务脚本、生产启动器或生产 Canary；
- 不承诺收益率、稳定盈利、机构级可靠性或数千级容量；
- 不把源码存在、历史测试或界面按钮当成真钱权限。

TAIL 当前以 Solana 研究和市场观察作为主要参考场景。其他市场只会在完成独立数据、规则、风险与执行验证后再讨论接入，不在本版本中提前承诺。

## 本次发布前验证

2026-09-04 的发布候选完成了以下检查：

- 159 个测试文件：158 通过、1 跳过；
- 2054 个测试：2049 通过、5 跳过；
- ESLint、TypeScript、服务端构建、Web 构建、桌面构建通过；
- 最终公开包烟雾测试退出码为 0；
- 解包审计仅包含 9 个应用文件，源码映射、研究任务脚本、生产启动器、生产 Canary、已知钱包地址、私人路径和疑似凭据均未检出；
- 两个 EXE 经本机 Microsoft Defender 扫描，结果均为未发现威胁。

这些结果只说明该发布候选在记录环境中的检查结果，不构成对所有设备、依赖或未来版本的保证。可复核清单见 [公开导出清单](PUBLIC-SCOPE.md) 与 [public-export-manifest.json](public-export-manifest.json)。

## 项目方向

TAIL 想解决的核心不是“再做一个会发订单的 Bot”，而是把下面这条链路做成可观察、可恢复、可核对的系统：

```text
Signal → Risk → Intent → Execute/Paper → Reconcile → Evidence → Recovery
```

真正困难的是：断线和重启后怎样恢复、重复事件怎样避免重复执行、状态不一致时相信哪一侧，以及发生异常后怎样知道下一步仍允许做什么。

## 旧版演示

约 52 秒的 0.0.1 早期视频仍保留在 [v0.0.1-preview](https://github.com/Tailovo/tail-trading-workspace/releases/tag/v0.0.1-preview)，仅作为历史记录。它的 UI 和状态不代表当前 0.4.1 预览。

## 许可证与反馈

当前仓库没有开源许可证。公开可见不代表允许复制、修改或再分发；安装包仅供评估本次早期预览。

普通问题与产品建议可通过 [GitHub Issues](https://github.com/Tailovo/tail-trading-workspace/issues) 提交。请勿上传私钥、助记词、Token、真实账户或未脱敏交易记录。安全问题请先阅读 [SECURITY.md](SECURITY.md)。

## 文档

- [0.4.1 发布说明](RELEASE-NOTES-0.4.1.md)
- [界面与功能导览](PRODUCT-TOUR.md)
- [当前状态](STATUS.md)
- [能力边界](CAPABILITIES.md)
- [平台架构](ARCHITECTURE.md)
- [路线图](ROADMAP.md)
- [规模与市场边界](SCALE-AND-MARKETS.md)
- [安全边界](SECURITY-BOUNDARY.md)
- [公开范围](PUBLIC-SCOPE.md)
- [开发日志](CHANGELOG.md)
- [反馈方式](FEEDBACK.md)

## 当前版本说明

现在看到的是 TAIL 的早期开发版本，不是最终成品。项目仍在持续开发，界面、交互、数据接入和功能边界都可能调整。
