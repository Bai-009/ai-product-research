# AI 技术架构研究、产品观察与演示影片

白东昊 · 基于真实产品逆向对照测试、前沿 AI Infra 架构拆解与工程落地实践。

---

## 一、四篇深度研究长文

| 篇 | 主题 | 核心内容 |
|---|---|---|
| **01** | [Vibe Coding 缺的不是发动机，而是方向盘：YouWare 产品观察与思考](./01-Vibe%20Coding%20缺的不是发动机而是方向盘：YouWare%20产品观察与思考.pdf) | 用两类提示词对 YouWare 与 Kimi Agent 做对照测试。五个发现指向同一件事：AI 缺乏判断边界，方向盘不是事后验货，而是在生成过程中持续校准方向。 |
| **02** | [用全覆盖代替精确度：Kimi 产品观察](./02-用全覆盖代替精确度：Kimi%20产品观察.pdf) | 从 Kimi 对不同模糊程度输入的反应，拆解「直接给结果」这一产品哲学及其代价：PPT、Agent、Kimi Claw 共享同一个隐含假设——用户在开始前就清楚自己要什么。 |
| **03** | [AI 不是终点：关于 AI 产品的思考和设计](./03-AI%20不是终点：关于%20AI%20产品的思考和设计.pdf) | AI 产品经理的使命、以 Claude 为例的「把用户当思考对手」、关系层优先于服务层、分代记忆与预编译、代劳的极限与 Agent 边界。 |
| **04** | [云端 Agent 与 Runtime 的新职责](./04-云端Agent与Runtime的新职责.md)（图文在线直读 · 含 6 张架构图） | 横向对标 OpenAI dots、Meta Muse、xAI Grok Bot、Claude Code 云端会话、Pi Durable 与 Tetral，拆解云端 Agent 的两层连续性、控制面与沙箱解耦，以及企业级云端 Agent Runtime（Astra）如何依托数据库经验解决中断恢复、调用幂等与交接冲突。 |

---

## 二、产品演示与技术机制影片

全部成品视频托管于本仓库 [GitHub Release · `videos-v1`](https://github.com/Bai-009/ai-product-research/releases/tag/videos-v1)（点击即可下载/播放）：

| 编号 | 影片 | 规格 | 核心看点 |
|---|---|---|---|
| **01** | [CanvasFlow · 工业备件采购比选（卡片讲解版）](https://github.com/Bai-009/ai-product-research/releases/download/videos-v1/01-CanvasFlow-Demo-Cards-4K.mp4)（[在线网页直看](https://canvasflow-matrixnext.vercel.app)） | 2m17s · 4K · 真人旁白+字幕 | 演示 CanvasFlow 接入 MOI CLI 与真实算子：从三份供应商 PDF 报价、关键规则澄清、按依赖逐节点构建与 Gate 校验，到真实运行输出 `supplier_comparison.csv` 与 `recommendation.json` 全链路闭环。 |
| **02** | [Silence · 云端 Agent 静默故障与外部 Loop 恢复](https://github.com/Bai-009/ai-product-research/releases/download/videos-v1/02-CloudAgent-Silence-Film-1080p.mp4) | 3m28s · 1080p · 英文配音+字幕 | 第 04 篇长文配套叙事影片：从本地迁云、42 项交叉依赖委托、凌晨沙箱静默失效，到控制面外置与跨环境接续恢复的完整机制呈现。 |
| **03** | [Astra · 执行前后各记录一次（Linear 动效样片）](https://github.com/Bai-009/ai-product-research/releases/download/videos-v1/03-Astra-Invocation-Journal-Linear-1080p.mp4) | 54s · 1080p · 配音+3D 动效 | 聚焦云端 Agent 工具调用的持久账本（Invocation Journal）、`Unknown` 不确定态与幂等防重设计，对应第 04 篇第五章核心机制。 |
| **04** | [Astra · 让优化有据可依（概念短片）](https://github.com/Bai-009/ai-product-research/releases/download/videos-v1/04-Astra-Context-Explain-1080p.mp4) | 40s · 1080p · 中文配乐概念片 | 借鉴数据库查询规划与 `EXPLAIN` 思路，直观呈现上下文组装、压缩取舍与运行过程可观测性。 |
| **05** | [LLM 前向推理全链路机制拆解](https://github.com/Bai-009/ai-product-research/releases/download/videos-v1/05-LLM-Forward-Pass-Explainer-1080p.mp4) | 5m21s · 1080p · 中文配音+可视化 | 第一性原理拆解大模型前向推理：切词、Embedding 查表、Causal Mask 与 Softmax 注意力、KV Cache 缓存复用与自回归采样。 |

---

## 三、关联开源项目与交互作品集

- **完整交互作品集（含交互原型与短片）**：[Bai-009/portfolio](https://github.com/Bai-009/portfolio)
- **CanvasFlow · AI 画布工作流**：[Bai-009/canvas-first-workflow](https://github.com/Bai-009/canvas-first-workflow)
- **Co-Thinker · 人机协同思考工作台**：[Bai-009/Co-Thinker](https://github.com/Bai-009/Co-Thinker)
- **Thinking · 智能体运行过程可观测 UI**：[Bai-009/agent-thinking-ui](https://github.com/Bai-009/agent-thinking-ui)
- **AI Agent 工程化题库复盘**：[Bai-009/agent-interview-notes](https://github.com/Bai-009/agent-interview-notes)

---

*Bai Donghao · Product studies, cloud agent runtime architecture essays, and product/mechanism demo films (2026).*
