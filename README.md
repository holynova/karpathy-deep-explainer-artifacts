# Karpathy AI Artifacts - 认知跃迁与深度工件实验室

> **"As LLMs get better, they will do more and more of the legwork autonomously, and a lot more of our work will rise up the abstractions into oversight and understanding... ask for large, custom, discardable software artifacts (e.g. web apps, video explainers). Push the boundaries here and you'll be surprised."**  
> — *Andrej Karpathy*

本项目基于 **Andrej Karpathy** 关于大模型输出形态演进的思考，深度结合 **Emil Kowalski** 的设计工程学（Design Engineering）与原型发散标准（Prototype Skill），全面清除 AI Slop（浮夸渐变、无意义霓虹发光、滥用 Emoji、空洞营销套话），打造高信噪比、具备真实触觉反馈与参数交互的专属软件工件。

---

## 🎨 设计工程学与去除 AI Slop 规范

本项目严格遵循 [Emil Kowalski 的 Design Engineering 与 Prototype 规范](https://github.com/emilkowalski/skills/blob/main/skills/prototype/SKILL.md)：

1. **去除常见 AI Slop**：
   - 移除无语义的彩虹渐变与刺眼高饱和度霓虹发光 (`box-shadow: 0 20px 40px ...`)，改用克制内敛的深色金属质感 (`#09090b`、1px 微细边框与 `inset 0 1px 0 0 rgba(255,255,255,0.04)` 微光)。
   - 彻底清除充斥于标题和按钮上的大量低质 Emoji，改用纯粹利落的几何符号与字体排印层级。
   - 剔除浮夸吹嘘的 AI 模板套话，回归扎实、严谨、以工程师为第一视角的系统语言。
2. **Emil Kowalski 标准的原型选择器 (The Floating Picker)**：
   - 底部悬浮深色磨砂玻璃胶囊 (`.proto-picker`)，搭载高精度的滑动高亮指示器 (`.proto-picker-highlight`)。
   - 使用定制缓动曲线 `--ease-out: cubic-bezier(0.23, 1, 0.32, 1)`，动效控制在 250ms 以内。
   - 键盘交互完整支持：数字键 `1-4`、左右方向键 `ArrowLeft`/`ArrowRight`、以及 `R` 键重放入场动画。
   - 页面状态持久化至 URL (`?v=1`..`?v=4`)，入场动画从 `scale(0.97)` 与 `opacity: 0` 平滑切入，严禁从 `scale(0)` 突兀放大。
3. **触觉反馈 (Tactile Responsiveness)**：
   - 所有可点击组件与按钮均实现 `:active { transform: scale(0.97); }` 即时按压反馈。

---

## 📚 5 大前沿专题空间与知识图谱

每个专题页面均为独立静态应用，内置 **10+ 个高级核心知识点**、严格的 **ASD-STE100 受控工程规约** 与 **工业级交互试验台**：

1. **前端系统设计 ([frontend-system-design.html](https://holynova.github.io/karpathy-deep-explainer-artifacts/frontend-system-design.html))**
   - 11 大核心知识点：微前端沙箱与 Module Federation 依赖去重、现代渲染时序瀑布流 (CSR/SSR/RSC/Islands)、Signals 细粒度响应、Local-First CRDT 离线同步、前端弹性自愈、全链路 RUM 与 LoAF 监控、Design Tokens 与 Headless 原语、海量数据虚拟滚动、Trusted Types 安全防御、INP `scheduler.yield()` 任务切片。
2. **系统设计与分布式架构 ([backend-system-design.html](https://holynova.github.io/karpathy-deep-explainer-artifacts/backend-system-design.html))**
   - 11 大核心知识点：Raft 共识与脑裂防御、PACELC 定理与延迟折衷、Saga 分布式事务与 Outbox CDC、LSM-Tree 存储分层压缩、缓存一致性与 Binlog 异步淘汰、一致性哈希虚拟节点、分布式限流算法、Kafka 分区并发与端到端 EOS、Full Jitter 削峰填谷、Snowflake 64位位运算、Dynamo Quorum 读写仲裁。
3. **提示词工程与认知架构 ([prompt-engineering.html](https://holynova.github.io/karpathy-deep-explainer-artifacts/prompt-engineering.html))**
   - 11 大核心知识点：动态 KNN 示例召回、Tree of Thoughts (ToT) 思维树剪枝、FSM 语法掩码确定性约束解码、DSPy MIPROv2 自动提示词优化、ReAct 工具异常反思自愈、上下文窗口 Lost-in-the-Middle 动力学、ASD-STE100 航空受控工程规约、间接注入防护与 Dual-LLM 沙箱、HyDE 假想文档生成、LLM-as-a-Judge 量表工程、LLMLingua 信息熵剪枝。
4. **Zara Zhang 的思想与认知模型 ([zara-zhang-insights.html](https://holynova.github.io/karpathy-deep-explainer-artifacts/zara-zhang-insights.html))**
   - 10 大核心心智模型："Build for One" 深度针对性、盆栽心态 (The Potted Plant Mindset)、软件作为人文叙事新媒介、反向学习 (Unlearning School) 摆脱好学生心态、"不实用就不是真精神追求"、写作即思考与内部清晰度、Humble AI 与高信噪比护城河、无阶梯的非线性职业生涯、中美科技产品哲学二元透视、偶然性接触面积与能动性肌肉。
5. **Matt Pocock: Engineering, Not Vibe Coding ([matt-pocock-insights.html](https://holynova.github.io/karpathy-deep-explainer-artifacts/matt-pocock-insights.html))**
   - 10 大核心工程原则："Engineering, Not Vibe Coding" 拒绝泥球债务雪崩、经典 "Grill Me" 需求反向质询技术、垂直切片与严格 TDD 导轨、白班人类规划与夜班 AI 交付模型、TypeScript 作为不可违背的物理护栏、Total TypeScript 知识民主化、定制化 Agent Skills 规范、共享设计共识 RFC、Branded Types 编译期防越权、从打字员到编排架构师的终极跃迁。

---

## 🚀 在线访问与本地运行

- **在线访问**：[https://holynova.github.io/karpathy-deep-explainer-artifacts/](https://holynova.github.io/karpathy-deep-explainer-artifacts/)
- **本地直接打开**：
  ```bash
  git clone https://github.com/holynova/karpathy-deep-explainer-artifacts.git
  cd karpathy-deep-explainer-artifacts
  open index.html
  ```

---

## 👤 致谢与参考标准
- **思想启发**：[Andrej Karpathy](https://twitter.com/karpathy)
- **设计工程标准与原型技能**：[Emil Kowalski](https://github.com/emilkowalski/skills)
- **工程构建**：[holynova](https://github.com/holynova)
