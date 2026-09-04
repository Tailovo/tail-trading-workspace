# TAIL

> 正在开发的 Solana 桌面交易工作台。

TAIL 从个人自用需求出发，探索把钱包观察、跟单研究和执行状态放进一个可追踪的工作流程。这里公开阶段成果、早期预览和下一步计划，也欢迎你分享实际使用场景。

**当前：0.4.1 · Windows x64 · 只读预览。** 可以体验桌面工作区、合成回测与固定样本浏览；公开包不接入真实钱包或实时行情，不提供真实交易能力。

[一分钟图文导览](PRODUCT-TOUR.md) · [下载当前预览](https://github.com/Tailovo/tail-trading-workspace/releases/tag/v0.4.1-preview) · [下一步计划](ROADMAP.md) · [分享一个需求](https://github.com/Tailovo/tail-trading-workspace/issues/new?template=product-feedback.yml)

![TAIL 0.4.1 运行总览：桌面工作区与右侧状态工具区，当前未连接实盘数据](assets/screenshots/tail-overview-v0.4.1.png)

## TAIL 想解决什么

观察钱包之后，为什么跟随或放弃？执行进展到哪一步？中断后怎样核对和继续？TAIL 希望把这些信息串起来，让研究过程和执行状态都有迹可循。

如果你在研究 Solana 钱包、尝试个人跟单工具，或关心自动化交易的状态与恢复问题，欢迎关注这个项目的验证过程。

## 当前可以体验什么

| 想先了解 | 在预览中看什么 |
| --- | --- |
| 工作流程怎样组织 | 分组导航、运行总览与可切换的右侧工具区 |
| 数据结果怎样呈现 | 运行内置合成回测，查看结果与数据来源标识 |
| 信息较多时怎样浏览 | 查看持仓固定样本的排列与滚动效果 |
| 工作区是否顺手 | 调整主题、背景、透明度及助手的位置和显示 |

合成回测与 Fixture（固定测试样本）用于展示界面和数据链路，不代表真实交易或收益。没有接入的数据会显示“未连接”或“暂不可用”。[按三步浏览当前界面 →](PRODUCT-TOUR.md)

## 下一次更新看什么

| 阶段 | 关注点 |
| --- | --- |
| 已公开 | 可运行的 Windows 桌面预览与当前界面导览 |
| 下一里程碑 | 从一条脱敏事件，追到每一步状态和最终证据的只读流程 |
| 随后验证 | 在模拟环境中处理重复事件、断线与重启，观察核对和恢复结果 |

下一里程碑的验收方式是：第一次使用的人也能从输入追到最终证据，看清哪些信息已知、哪些仍然缺失。它是下一步计划，尚未作为本次公开包的完整能力交付。进展以验证结果为准，[查看完整路线图](ROADMAP.md)。

## 下载 Windows 预览

| 版本 | 适合场景 | 下载 |
| --- | --- | --- |
| 安装版 | 安装到当前 Windows 用户 | [TAIL-V0.4.1-Preview-Setup-x64.exe](https://github.com/Tailovo/tail-trading-workspace/releases/download/v0.4.1-preview/TAIL-V0.4.1-Preview-Setup-x64.exe) |
| 便携版 | 不安装，直接运行单个 EXE | [TAIL-V0.4.1-Preview-Portable-x64.exe](https://github.com/Tailovo/tail-trading-workspace/releases/download/v0.4.1-preview/TAIL-V0.4.1-Preview-Portable-x64.exe) |

**下载前请了解：** 这是早期只读预览，没有钱包连接、签名、广播、真实下单或自动卖出能力。EXE 尚未进行 Authenticode 代码签名，Windows 可能显示未知发布者或 SmartScreen 提示。请只从本仓库 Release 下载，并核对 [SHA256SUMS.txt](https://github.com/Tailovo/tail-trading-workspace/releases/download/v0.4.1-preview/SHA256SUMS.txt)。

0.4.1 发布候选已记录构建、测试、包内容审计与烟雾检查结果；这些是该候选的验证记录，不构成安全或收益保证。[发布说明与校验值](RELEASE-NOTES-0.4.1.md) · [公开范围与发布检查](PUBLIC-SCOPE.md) · [安全边界](SECURITY-BOUNDARY.md)

## 参与和关注

- **分享场景：** [说说你希望 TAIL 帮你解决什么问题](https://github.com/Tailovo/tail-trading-workspace/issues/new?template=product-feedback.yml)，可以只写一个具体场景，无需准备测试报告。
- **体验反馈：** [报告安装或界面问题](https://github.com/Tailovo/tail-trading-workspace/issues/new?template=preview-bug.yml)，或先查看[反馈指南](FEEDBACK.md)。
- **关注进展：** 用 Star 收藏项目；需要版本通知时，可在 GitHub 的 Watch → Custom 中选择 Releases。[开发日志](CHANGELOG.md)会说明每次公开更新的内容。

请勿在公开反馈中提交凭据、真实账户或未脱敏交易记录。安全问题见 [SECURITY.md](SECURITY.md)；目前尚未提供独立的保密安全联系渠道。

## 进一步了解

[当前状态](STATUS.md) · [能力边界](CAPABILITIES.md) · [平台架构](ARCHITECTURE.md) · [规模与市场边界](SCALE-AND-MARKETS.md)

当前仓库用于公开展示和早期预览，未开放私有主项目源码，也没有开源许可证。安装包仅供评估本次预览；公开可见不代表允许复制、修改或再分发。界面、交互和数据接入会随验证继续调整。
