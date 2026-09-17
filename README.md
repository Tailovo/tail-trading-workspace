# TAIL

**个人借助 AI 开发的 Solana 桌面跟单与交易状态工作台。**

从自己的使用需求出发，我使用 Codex 推进 TAIL 的需求拆解、技术实现、运行验证和迭代。项目把来源钱包事件、跟随执行、持仓和最终对账放在同一个桌面工作区，持续处理真实运行中暴露的问题。

**项目进展更新：2026-09-17。公开下载仍为 `v0.4.1-preview`，只提供只读体验。** 私有开发版已出现真实自动买卖闭环成功案例，当前重点是来源监听恢复、事件顺序与执行延迟。历史成功不代表当前版本已经持续稳定运行。

[界面导览](PRODUCT-TOUR.md) · [Windows 只读预览](https://github.com/Tailovo/tail-trading-workspace/releases/tag/v0.4.1-preview) · [当前架构](ARCHITECTURE.md) · [工程与 AI 协作](docs/ENGINEERING.md) · [当前状态](STATUS.md)

![TAIL 开发界面运行总览，2026-09-17 隔离空会话截图，未连接交易服务](assets/screenshots/development-2026-09-17/overview.png)

上图是当前开发界面在隔离截图环境中的实际渲染，使用空会话测试桥接；它不代表公开安装包已更新，也不代表当前存在真实持仓或交易。全部页面与截图来源见[界面导览](PRODUCT-TOUR.md)。

## 产品现在做到了哪里

| 范围 | 已有成果 | 当前限制 |
| --- | --- | --- |
| 公开下载版 | Windows 安装版与便携版、工作区、合成回测、固定样本、个性化 | 2026-09-04 的只读预览，无真实交易能力 |
| 私有开发版 | 会话配置、来源动作路由、逐仓执行、预算与持仓读模型；历史自动买卖闭环案例 | 来源恢复与延迟仍在处理，多仓持续实盘表现未完成验证 |
| 本次公开更新 | 11 张开发界面截图、当前调用架构、工程案例、更新后的路线图 | 文档与截图更新，不是新安装包发布 |

## 想解决的具体问题

- 跟随来源交易时，看清事件进入、执行与对账分别到了哪一步。
- 发生中断时，保留持仓、未决交易和来源状态，避免把“已提交”误当成“已成交”。
- 将一个仓位和多个仓位放在可复用的会话、路由与执行结构中，逐步验证容量。
- 让实际运行问题有记录、可以复现，并能判断一次修改是否改善了目标行为。

## 项目实现与个人贡献

项目使用 **TypeScript、Electron、React / Next.js、Node.js / Fastify**，并集成 Solana 数据与交易接口。技术栈描述项目实现，不表示所有底层代码均为本人独立编写。

我负责产品目标、使用场景、运行反馈与结果验收，借助 Codex 推进技术方案、编码、测试和交付。大量实现由 AI 参与完成；设计与实现结论通过代码、运行记录和针对性验证核对。[查看具体工作方式与工程案例](docs/ENGINEERING.md)。

当前仓库公开产品资料、截图和预览安装包，**主项目源码暂未开放**。架构说明和工程记录不能替代公开可运行源码；可公开代码范围仍待整理。

## 下载与体验

| Windows x64 | 下载 |
| --- | --- |
| 安装版 | [TAIL 0.4.1 Preview Setup](https://github.com/Tailovo/tail-trading-workspace/releases/download/v0.4.1-preview/TAIL-V0.4.1-Preview-Setup-x64.exe) |
| 便携版 | [TAIL 0.4.1 Preview Portable](https://github.com/Tailovo/tail-trading-workspace/releases/download/v0.4.1-preview/TAIL-V0.4.1-Preview-Portable-x64.exe) |

公开包不连接真实钱包、不签名、不广播、不执行买卖。EXE 未进行 Authenticode 代码签名；从本仓库 Release 下载，并核对 [SHA256SUMS.txt](https://github.com/Tailovo/tail-trading-workspace/releases/download/v0.4.1-preview/SHA256SUMS.txt)。[原版本发布说明](RELEASE-NOTES-0.4.1.md)保留该版本的历史验证记录。

## 下一步

优先完成当前来源会话的恢复与顺序处理，记录来源事件到执行确认的分段耗时，再验证相同核心在不同仓位容量下的表现。公开展示复用已有界面与只读实现，不另外建立一套交易引擎。[具体里程碑](ROADMAP.md)。

[提交体验问题](https://github.com/Tailovo/tail-trading-workspace/issues/new?template=preview-bug.yml) · [分享使用场景](https://github.com/Tailovo/tail-trading-workspace/issues/new?template=product-feedback.yml) · [开发日志](CHANGELOG.md)

公开内容没有授予开源许可证；使用范围见[公开范围](PUBLIC-SCOPE.md)，敏感问题见 [SECURITY.md](SECURITY.md)。
