# TAIL 0.4.1 界面导览

以下截图来自当前候选包或同一候选源码的 UI Harness。状态、合成样本和 Fixture 均按原样标注，不代表真实账户或实时市场。

## 运行总览

主工作区取消了旧式大卡片堆叠，改成更连续的信息层级；左侧使用分组导航，右侧保留可切换工具区。

![TAIL 运行总览](assets/screenshots/tail-overview-v0.4.1.png)

## 行情与 K 线工具区

右侧可以切换到行情与 K 线模式。公开包不携带可核实行情源，因此图中如实显示暂不可用。

![TAIL 行情与 K 线工具区](assets/screenshots/tail-market-panel-v0.4.1.png)

## 内置研究浏览器

浏览器工具区提供独立的 HTTPS 研究入口，并显示隔离配置。截图没有主动打开远程页面。

![TAIL 内置浏览器](assets/screenshots/tail-browser-panel-v0.4.1.png)

## 公开研究工作台

公开构建保留研究工作流的产品表面，但私有研究任务脚本被物理排除，按钮保持只读。

![TAIL 公开研究工作台](assets/screenshots/tail-research-public-preview-v0.4.1.png)

## 合成回测

数据分析页可以运行内置合成样本，结果区域明确写明“合成样本”，只验证界面与数据链路，不证明收益。

![TAIL 合成回测](assets/screenshots/tail-backtest-synthetic-v0.4.1.png)

## 持仓 Fixture

100 条持仓是用于布局和滚动验证的固定 Fixture，界面明确标注 TEST / FIXTURE，不是用户账户数据。

![TAIL 持仓 Fixture](assets/screenshots/tail-positions-fixture-v0.4.1.png)

## 个性化与助手

设置页保留背景、透明度、颜色、减少动画和助手显示/位置等本地偏好。这些设置不会改变交易、签名或广播权限。

![TAIL 个性化设置](assets/screenshots/tail-personalization-v0.4.1.png)

## 后端断连状态

当本地产品状态不可核实时，系统页显示未连接与等待状态，不使用历史值填充。

![TAIL 后端断连状态](assets/screenshots/tail-system-offline-v0.4.1.png)

## 历史视频

[v0.0.1-preview 的约 52 秒视频](https://github.com/Tailovo/tail-trading-workspace/releases/download/v0.0.1-preview/tail-early-preview-2026-09-01.mp4) 保留为历史记录。视频中的旧 UI 不代表当前 0.4.1。

当前仍不是最终版本。界面、交互、数据接入和能力边界会继续调整。
