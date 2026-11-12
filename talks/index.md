[返回首页](../README.md)

# Day 1 选看索引

可以按正在做的事挑场次，也可以在每场下面按时间跳到对应段落。Natalie 一场分别标出补录和原录屏的时间，其余场次对应原录屏。

## 按主题挑场次

**想看 Agent 真正进入团队以后发生什么**

[Joey Wang](#talk-06) · [Chinmay Gandhi、Swaapnika Motapothula、Vlad Tsvang](#talk-08) · [Zach Bruggeman](#talk-25)

**想把代码审查、测试和恢复做扎实**

[Lauren Tan](#talk-04) · [Andrew Finch](#talk-11) · [Kush Agrawal](#talk-15) · [Tanmay Sah、Dolly Sah](#talk-14)

**正在改 Harness、Skill 或多 Agent 编排**

[Philipp Schmid](#talk-09) · [Nikolay Petrov](#talk-23) · [Girish Konda](#talk-22) · [Luke Alvoeiro](#talk-12)

**想把推理、产品交互和快速判断连起来**

[Natalie Serrino](#talk-01) · [Michelle Chen](#talk-03) · [Chinmay Goyal](#talk-18) · [Scott Roberts](#talk-21)

**先补全年视角，再看新工具的来路**

[Simon Willison](#talk-27) · [Steve Yegge](#talk-26) · [Lydia Hallie](#talk-02)

## 录屏与官方资料

本索引覆盖原录屏和 Natalie 的补录。Lydia 现场遇到设备故障，Roey 的插播中途切出，Philipp 开场音频难辨。对应条目附有可用的官方入口。

[AIE 官方议程](https://ai.engineer/code/2026/schedule) · [讲者资料](https://ai.engineer/code/2026#speakers) · [Day 1 官方回放](https://www.youtube.com/watch?v=ZZ19zhYnDKY)

## 全部场次

<a name="talk-01"></a>

### 01 · What Will You Build When AI Is 10x Faster?

**Natalie Serrino** · Gimlet Labs · Co-Founder

参与构建用 AI 生成和优化推理内核的 KForge。

Natalie 先用 Figma 和早期网页邮箱演示等待怎样打断工作，再用小游戏说明推理速度和吞吐量为何会互相制约。她接着展示混用不同类型芯片、减少端到端等待的做法，并以实时防护演示说明延迟为何会改变产品能做的事。

- [补录 00:00:06](01-natalie-serrino.md#section-1) 开场、自我介绍和 Figma 改幻灯片演示
- [补录 00:01:29](01-natalie-serrino.md#section-2) 网页邮箱对照、用户等待和 63 秒 Agent 回合
- [补录 00:03:02](01-natalie-serrino.md#section-3) 算力约束、Token Mint Factory 和速度与吞吐量的取舍
- [补录 00:04:05](01-natalie-serrino.md#section-4) 异构推理、贪吃蛇演示和工具调用瓶颈
- [补录 00:06:10](01-natalie-serrino.md#section-5) 普通速度和超低延迟的防护对照
- [补录 00:07:37](01-natalie-serrino.md#section-6) 从网页邮箱到高清串流，再谈实时交互
- [原录屏 00:02:43](01-natalie-serrino.md#section-7) 交互补全、更多智能体和致谢

补录 00:00:06–00:08:17  ·  原录屏 00:02:43–00:03:26 · 34 张图 · [打开中英对照稿](01-natalie-serrino.md)

[Gimlet Labs 技术博客](<https://gimletlabs.ai/blog>) · [官方回放](<https://www.youtube.com/watch?v=ZZ19zhYnDKY&t=687s>)

<a name="talk-02"></a>

### 02 · Rethinking Claude Code Best Practices

**Lydia Hallie** · Anthropic · Member of Technical Staff

负责 Claude Code 开发者关系，也是 JavaScript Visualized 系列作者。

Lydia 在现场设备故障期间提到，能自行验证的模型可以在云端连续工作数小时，人参与 Claude Code 会话的方式也随之改变。要听整场，请从她后来重录的 AIE 单场视频开始。

- [00:04:52](02-lydia-hallie.md#section-1) 与观众聊 Fable 和 Opus 的使用场景
- [00:08:48](02-lydia-hallie.md#section-2) 临场谈长时间云端会话、模型自验与人的角色
- [00:09:55](02-lydia-hallie.md#section-3) 排障和现场交流，随后结束

录屏 00:04:09–00:13:13 · 8 张图 · [打开中英对照稿](02-lydia-hallie.md)

[JavaScript Visualized 系列](<https://dev.to/lydiahallie/series>) · [AIE 完整重录版](<https://www.youtube.com/watch?v=vlfCjWuv4es>)

<a name="talk-03"></a>

### 03 · cloudflare is a neolab

**Michelle Chen** · Cloudflare · Group Product Manager

负责 Cloudflare AI 平台的产品工作，并参与发布 Clef 和 Clairic。

Cloudflare 从 CDN 做到边缘计算、存储和模型推理。Michelle 用 CI 故障分诊演示如何把可枚举的判断交给小模型，把需要阅读日志或综合证据的部分留给大模型。

- [00:16:30](03-michelle-chen.md#section-1) CDN、Workers、存储和模型服务的演进
- [00:23:04](03-michelle-chen.md#section-2) Jev、Clef、Clairic 与 System One 判断
- [00:28:45](03-michelle-chen.md#section-3) 分诊失败的 CI，比较大模型调用与混合流程

录屏 00:15:03–00:34:53 · 37 张图 · [打开中英对照稿](03-michelle-chen.md)

[Cloudflare 发布 Clairic](<https://blog.cloudflare.com/clairic-extraction-model/>)

<a name="talk-04"></a>

### 04 · All Code Is Slop (Except Mine)

**Lauren Tan** · SpaceXSI · Principal Engineer

参与 Grok Bot 和客户端架构。

Lauren 从团队大量合并 PR 的经历出发，讨论怎样让工程师敢于放手。她把清楚的代码结构、静态检查、运行时验证和交付流程放在同一张图里，并用团队的产出和回退数据解释取舍。

- [00:36:50](04-lauren-tan.md#section-1) PR 规模与信任如何制约并行
- [00:38:27](04-lauren-tan.md#section-2) 用代码结构和静态检查减少重复踩坑
- [00:46:06](04-lauren-tan.md#section-3) 运行时验证、形式化验证和 UI 测试
- [00:49:43](04-lauren-tan.md#section-4) PR 产出、回退率与软件工厂的适用条件

录屏 00:35:56–00:53:34 · 47 张图 · [打开中英对照稿](04-lauren-tan.md)

<a name="talk-05"></a>

### 05 · KV-first Security

**Ari Azarafrooz** · Intrinsec AI · Founder

Ari 讨论如何从推理引擎已产生的 KV cache 寻找异常信号。语音智能体案例展示了怎样定位异常片段，文本案例接着讨论误报、模型换代和 KV 数据传输的成本。

- [01:05:35](05-intrinsec.md#section-1) KV cache 可以补充哪些现有防护信号
- [01:07:41](05-intrinsec.md#section-2) 基线、异常检测及推理栈中的接入位置
- [01:09:37](05-intrinsec.md#section-3) 语音与文本场景的案例及部署难点

录屏 01:05:34–01:12:46 · 5 张图 · [打开中英对照稿](05-intrinsec.md)

<a name="talk-06"></a>

### 06 · 10,000 agent PRs later, what broke wasn’t the agents

**Joey Wang** · Harvey · Engineering Lead

负责后台 Agent，曾联合撰写 Harvey 的 Spectre 架构文章。

Harvey 让 Claude Code、Cursor 等前端共享一套内部云端执行和交付流程。当同一告警拉起大量任务、单个用户占满集群、合并开始排队时，团队修的是触发、调度和合并这几段。

- [01:13:07](06-joey-wang.md#section-1) 超过一万个 Agent PR 后，平台成了瓶颈
- [01:15:20](06-joey-wang.md#section-2) Spectre 如何串起代码、环境、验证和交付
- [01:18:07](06-joey-wang.md#section-3) 人和 Agent 都能发起任务，入口与使用习惯怎样变化
- [01:20:25](06-joey-wang.md#section-4) 告警风暴、集群公平调度、合并队列

录屏 01:12:46–01:25:39 · 29 张图 · [打开中英对照稿](06-joey-wang.md)

[Building Spectre](<https://www.harvey.ai/blog/building-spectre-internal-collaborative-cloud-agent-platform>)

<a name="talk-07"></a>

### 07 · Specs Have Bugs Too

**Rajath Kotyal** · Amazon Web Services · Software Developer II

两条单看都合理的库存规则，放在一起可能同时要求接受和拒绝同一订单。Rajath 让 LLM 把规格转成逻辑表达，再用求解器寻找冲突和缺口，最后让人确认含义。

- [01:25:50](07-rajath-kotyal.md#section-1) 订单规则为何产生歧义
- [01:28:36](07-rajath-kotyal.md#section-2) LLM 翻译规格，SMT 求解器检查
- [01:29:51](07-rajath-kotyal.md#section-3) 对多种解释做聚类，定位冲突与遗漏
- [01:31:56](07-rajath-kotyal.md#section-4) 方法边界以及交给工程师的复核问题

录屏 01:25:39–01:33:31 · 12 张图 · [打开中英对照稿](07-rajath-kotyal.md)

<a name="talk-08"></a>

### 08 · 3 Levels of Autonomy: Building an AI On-Call Teammate at Meta

**Chinmay Gandhi** · Meta · Sr. Engineering Manager

**Swaapnika Motapothula** · Meta · Software Engineer

**Vlad Tsvang** · Meta · Software Engineer

Meta 团队用一次深夜告警展示值班 Agent 能接手哪些工作。权限分三个阶段，从按需建议，到经人批准后执行，再到给定范围内自主行动。不同团队共享基础能力，也保留各自的值班经验。

- [01:33:53](08-meta-on-call.md#section-1) 发布更快以后，值班仍要拼接零散信号
- [01:38:45](08-meta-on-call.md#section-2) 三档自主权与人需要介入的地方
- [01:42:05](08-meta-on-call.md#section-3) 告警示例、自动化和共享 Agent
- [01:45:37](08-meta-on-call.md#section-4) 团队定制、值班反馈和后续计划

录屏 01:33:31–01:49:10 · 18 张图 · [打开中英对照稿](08-meta-on-call.md)

<a name="talk-09"></a>

### 09 · I deleted 90% of my harness (And It Got Better)

**Philipp Schmid** · Google DeepMind · Member of the Technical Staff

从事 Gemini 和 Gemma 的开发者工作，曾任 Hugging Face 技术负责人。

Philipp 用同一类任务比较多工具 Harness 与只给模型一个 Bash 工具的实现。他展示调用数、token 消耗和任务分数，并讨论模型换代后可以重新验证哪些编排逻辑。

- [01:56:11](09-philipp-schmid.md#section-1) 模型变化与 Gemini Decisions API
- [01:58:57](09-philipp-schmid.md#section-2) 四次重做 Harness，从显式流程到一个工具
- [02:02:21](09-philipp-schmid.md#section-3) 同模型同任务的调用比较与评测
- [02:05:12](09-philipp-schmid.md#section-4) 实机演示及如何衡量每个已解决任务的成本

录屏 01:55:35–02:11:51 · 27 张图 · [打开中英对照稿](09-philipp-schmid.md)

[Philipp Schmid 技术博客](<https://www.philschmid.de/>)

<a name="talk-10"></a>

### 10 · The Rise of the Agent Workforce: Rethinking Agent Infrastructure

**Ankit Mathur** · Databricks · Member of Technical Staff

负责 Databricks 的 AI 基础设施工程。

Ankit 用多分支搜索说明，Agent 越能并行探索，越需要可复制的真实工作环境。他从生产数据管线举例，把分支能力延伸到会话、记忆、存储和整个工作状态。

- [02:21:30](10-ankit-mathur.md#section-1) 从棋局多路径搜索讲到团队型 Agent
- [02:24:26](10-ankit-mathur.md#section-2) 用分支和模拟验证真实工作流
- [02:28:20](10-ankit-mathur.md#section-3) 对会话、记忆和沙箱文件系统建分支
- [02:35:12](10-ankit-mathur.md#section-4) 用安全事件调查展示如何保留独立证据和推理分支

录屏 02:21:29–02:38:06 · 34 张图 · [打开中英对照稿](10-ankit-mathur.md)

<a name="talk-11"></a>

### 11 · Building a Safe Software Factory

**Andrew Finch** · Sonar · Staff Software Engineer

参与构建 Sonar 的 AI 代码审查产品 Gitar。

Andrew 把软件工厂拆成合并前验证、上线后验证、定期维护和知识反馈。讲到 PR 时，他展开了需要提交哪些证据，团队又如何逐步放开自动合并。

- [02:46:31](11-andrew-finch.md#section-1) 从软件交付瓶颈引出验证回路
- [02:49:18](11-andrew-finch.md#section-2) PR 验证、扩展审查范围与合并门槛
- [02:54:18](11-andrew-finch.md#section-3) 上线后复查、定期扫描和维护
- [02:56:40](11-andrew-finch.md#section-4) 把审查发现反馈给编码 Agent

录屏 02:45:07–02:59:27 · 33 张图 · [打开中英对照稿](11-andrew-finch.md)

<a name="talk-12"></a>

### 12 · Earning Autonomy: From Missions to Workstreams

**Luke Alvoeiro** · Factory · Member of Technical Staff

负责 Factory 的核心 Agent，参与构建 Droid 和 Missions。

Factory 的 Missions 需要先定计划，范围一变就容易反复交接。Luke 介绍如何把这种一次性任务变成长期 Workstream，让 Agent 围绕同一目标分工，再按验证信号逐步减少人工确认。

- [03:18:32](12-luke-alvoeiro.md#section-1) 软件工厂的组成及 Missions 的实际摩擦
- [03:21:31](12-luke-alvoeiro.md#section-2) 调度、计算隔离和程序化工具调用
- [03:25:04](12-luke-alvoeiro.md#section-3) Workstream 如何接任务、分工和累积上下文
- [03:29:22](12-luke-alvoeiro.md#section-4) 合并门槛、返工信号与逐步放权

录屏 03:17:40–03:33:27 · 31 张图 · [打开中英对照稿](12-luke-alvoeiro.md)

<a name="talk-13"></a>

### 13 · Recursively Self-Improvement for Coding Agents

**Ara Khan** · Cline · Founding Engineer

Cline 让一个 Agent 针对评测中暴露的失败改另一个 Agent 的 Harness。限流退避、误报循环和进程提前退出都是实在的工程问题。Ara 再讨论怎样用固定测试、人审和可重复的验证保住改进证据。

- [03:39:26](13-ara-khan.md#section-1) 递归自我改进的含义及编码 Agent 的演进
- [03:42:50](13-ara-khan.md#section-2) Agent 评测、Terminal-Bench 和迭代流程
- [03:46:23](13-ara-khan.md#section-3) Cline 实验、具体修复及验证方式
- [03:49:18](13-ara-khan.md#section-4) 推理、训练、现实世界任务和职业建议

录屏 03:34:34–04:01:12 · 40 张图 · [打开中英对照稿](13-ara-khan.md)

<a name="talk-14"></a>

### 14 · The Missing Undo Button for Coding Agents

**Tanmay Sah** · Independent · AI Researcher

**Dolly Sah** · Independent · Analyst

任务做完与失败后能恢复，是两项可以分别评测的能力。Tanmay 和 Dolly 用超时场景区分重试、回滚和补偿，再展示怎样在允许改动前验证恢复路径。

- [04:01:48](14-tanmay-and-dolly-sah.md#section-1) 完成任务与恢复状态的差距
- [04:03:40](14-tanmay-and-dolly-sah.md#section-2) 超时是否已经产生副作用，Git 能还原哪些状态
- [04:08:20](14-tanmay-and-dolly-sah.md#section-3) UndoBench、失败归因和恢复方法对照
- [04:11:56](14-tanmay-and-dolly-sah.md#section-4) EvoUndo 的状态取证、恢复演示和放行条件

录屏 04:01:12–04:17:48 · 23 张图 · [打开中英对照稿](14-tanmay-and-dolly-sah.md)

<a name="talk-15"></a>

### 15 · How AI Agents Shipped over 200k Lines of Tests on a 1.8M Line Codebase

**Kush Agrawal** · Duolingo · Staff Software Engineer

Duolingo 从本地批量验证起步，为 iOS 代码库搭起定时补测试的流水线。Kush 展示如何选文件、生成测试、修 CI、找审查人，并给出团队报告的合并量和覆盖率。

- [04:18:20](15-kush-agrawal.md#section-1) iOS 代码规模、初始覆盖率和为何优先补单测
- [04:21:40](15-kush-agrawal.md#section-2) 本地批次、文件评分和定时补测
- [04:25:12](15-kush-agrawal.md#section-3) PR 生命周期、自动修 CI 和质量门槛
- [04:28:49](15-kush-agrawal.md#section-4) 合并与覆盖率结果，以及可以迁移的流程

录屏 04:17:48–04:30:26 · 45 张图 · [打开中英对照稿](15-kush-agrawal.md)

<a name="talk-16"></a>

### 16 · What Happens When You Detonate Thousands of Agent Skills?

**Roey Ben Chaim** · Zenity &amp; MATS Fellowship · Staff Engineer &amp; AI Security Researcher

Roey 用一个授权诊断工具说明，乍看可疑的动作需要结合任务和执行环境判断。他介绍在隔离环境中记录 Agent 使用 Skill 的轨迹，录屏在单场视频中途切出。

- [04:30:28](16-roey-ben-chaim.md#section-1) Skill 带来的能力及其信任问题
- [04:32:05](16-roey-ben-chaim.md#section-2) 静态检查的局限与隔离观测思路
- [04:33:24](16-roey-ben-chaim.md#section-3) 沙箱运行、环境依赖与任务覆盖

录屏 04:30:27–04:36:17 · 15 张图 · [打开中英对照稿](16-roey-ben-chaim.md)

[AIE 单场回放](<https://www.youtube.com/watch?v=_7P580m4kPY>)

<a name="talk-17"></a>

### 17 · I love you so jevving much

**Diogo Almeida** · TypeSafe AI · Co-founder &amp; CEO

正在构建返回结构化判断和概率的 Jev。

Diogo 区分人与 AI 协作时的开放式生成，以及流程里需要可预测结果的自动判断。他用 Jev 讨论怎样把判断做成返回类型和概率的组件，再展望实时安全与生成式界面。

- [04:42:00](17-diogo-almeida.md#section-1) 为什么辅助能力强，自动化仍有缺口
- [04:47:30](17-diogo-almeida.md#section-2) 训练目标、可靠判断及 Jev 的产品定位
- [04:54:01](17-diogo-almeida.md#section-3) 从判断组件到软件工程中的新组合
- [05:00:12](17-diogo-almeida.md#section-4) 实时判断、语义类型和交互界面的设想

录屏 04:41:36–05:04:48 · 39 张图 · [打开中英对照稿](17-diogo-almeida.md)

<a name="talk-18"></a>

### 18 · Beyond Generation: Fast, Structured AI Decisions with Jev at Glean

**Chinmay Goyal** · Glean · Software Engineer

负责 Glean Assistant 和 Agent 相关工作。

Glean 把搜索和助手里原来交给生成模型的有界判断拆开测试。Chinmay 展示查询分类、路由、建议排序、引用校验和防护判断，并说明模型不确定时怎样回退。

- [05:10:08](18-chinmay-goyal.md#section-1) 识别输出可枚举的任务，介绍评测流程
- [05:12:59](18-chinmay-goyal.md#section-2) 查询分类、专家路由和建议排序
- [05:18:28](18-chinmay-goyal.md#section-3) 置信度、引用校验和防护判断
- [05:23:45](18-chinmay-goyal.md#section-4) 怎样选择决策模型、规则或生成模型

录屏 05:09:27–05:25:04 · 14 张图 · [打开中英对照稿](18-chinmay-goyal.md)

<a name="talk-19"></a>

### 19 · Your Automation Is Overthinking It

**Chibi Vikram** · UiPath · Engineer

**Kevin Bernstein** · UiPath · Principal AI Solution Architect

UiPath 用银行交易的虚构演示说明如何让快速模型并行初筛，再把值得调查的少数记录交给多步流程。后半场把同样的思路应用到检索重排和邮件结构化。

- [05:29:35](19-chibi-vikram-kevin-bernstein.md#section-1) Jev 在 Maestro 流程中的位置
- [05:31:10](19-chibi-vikram-kevin-bernstein.md#section-2) 可疑交易初筛与后续调查演示
- [05:34:35](19-chibi-vikram-kevin-bernstein.md#section-3) 分类、路由等用法及检索重排
- [05:38:36](19-chibi-vikram-kevin-bernstein.md#section-4) 从邮件挖掘结构化数据，比较示例延迟和成本

录屏 05:27:09–05:41:50 · 31 张图 · [打开中英对照稿](19-chibi-vikram-kevin-bernstein.md)

<a name="talk-20"></a>

### 20 · Your Judge Is Hallucinating Too

**Brian Kennedy** · ZoomInfo · Principal Engineer

负责 ZoomInfo 的 Agentic AI 平台工程。

Agent 声称邮件已经排程，裁判判了通过，但工具只创建了待办。Brian 以这个生产案例说明为什么验收要查工具证据，然后展示用结构化小判断替代部分裁判任务的离线对比和影子运行。

- [05:46:06](20-brian-kennedy.md#section-1) 失败样本与通用裁判的职责
- [05:55:12](20-brian-kennedy.md#section-2) 500 条生产步骤的离线评测及误收分析
- [05:57:25](20-brian-kennedy.md#section-3) 让模型针对工具结果回答更小的问题
- [06:00:37](20-brian-kennedy.md#section-4) 影子评测、后置条件及上线前验证

录屏 05:45:25–06:03:05 · 27 张图 · [打开中英对照稿](20-brian-kennedy.md)

<a name="talk-21"></a>

### 21 · Autocomplete for Actions: System One from the UI to the DB

**Scott Roberts** · Workday · Principal Engineer

Workday 把文字补全改成动作补全。用户还在输入时，系统就能判断是请假、看工资条还是约会，并打开相应界面。Scott 后面用招聘检索展示如何在查询中直接调用自然语言判断。

- [06:05:04](21-scott-roberts.md#section-1) 哪些交互能用快速分类完成
- [06:09:14](21-scott-roberts.md#section-2) 从补全词语到补全动作，展示产品界面
- [06:12:00](21-scott-roberts.md#section-3) 延迟、路由和不同团队维护规则的办法
- [06:13:15](21-scott-roberts.md#section-4) 招聘检索、SQL 里的自然语言判断和演示

录屏 06:04:51–06:16:53 · 34 张图 · [打开中英对照稿](21-scott-roberts.md)

<a name="talk-22"></a>

### 22 · Sub-Agents Are a Distributed System (And Nobody Gave You a Consistency Model)

**Girish Konda** · Microsoft · Principal Software Engineer

多个子 Agent 共用上下文并交接结果，会遇到部分失败、重复副作用和并发写入。Girish 用分布式系统的例子，介绍怎样给交接结果附上出处、状态和可执行的验证条件。

- [06:18:49](22-girish-konda.md#section-1) 把编排器、子 Agent 与共享状态画成分布式系统
- [06:19:51](22-girish-konda.md#section-2) 部分失败、脏读、扇出与重试
- [06:27:09](22-girish-konda.md#section-3) 选择一致性约束，介绍 SAFE 交接
- [06:29:43](22-girish-konda.md#section-4) 来源、幂等、隔离、并发边界及代码验证

录屏 06:18:00–06:40:56 · 38 张图 · [打开中英对照稿](22-girish-konda.md)

<a name="talk-23"></a>

### 23 · Your SKILL.md is 70% of Things the Model Already Knows

**Nikolay Petrov** · Intel · AI Engineering Manager

Nikolay 把 Skill 拆成可测试的小条目，对同一个问题分别带和不带 Skill 作答，再检查模型原来就懂什么、学到什么、是否受到了干扰。保留条文的决定还要看实际任务效果。

- [06:41:15](23-nikolay-petrov.md#section-1) 区分 Skill 传授知识和约束行为的作用
- [06:44:14](23-nikolay-petrov.md#section-2) 把条目拆成问题并做有无 Skill 的对照
- [06:48:40](23-nikolay-petrov.md#section-3) 冲突条款、已有知识和不同 Skill 的差异
- [06:53:11](23-nikolay-petrov.md#section-4) 用新信息量找实验方向，并用任务评测复核

录屏 06:40:56–06:54:57 · 14 张图 · [打开中英对照稿](23-nikolay-petrov.md)

<a name="talk-24"></a>

### 24 · What it takes to set intelligence free

**Fabian Hedin** · Lovable · CTO

Lovable 联合创始人，现任 CTO。

Lovable 从早期 Agent 尝试退回过简单调用链，后来又重新引入长任务。Fabian 展示怎样把任务历史放到进程外，用快照保存运行环境，再用验证结果决定当场修复或交给长期改进。

- [07:07:38](24-fabian-hedin.md#section-1) 从 GPT Engineer、早期 Agent 框架到聊天加预览
- [07:14:05](24-fabian-hedin.md#section-2) 十小时级任务所需的运行时、计算环境和验证
- [07:15:16](24-fabian-hedin.md#section-3) 事件历史、任务分支、回放和跨部署接续
- [07:20:41](24-fabian-hedin.md#section-4) 计算快照、共享内存、预览优化和双重验证回路

录屏 07:06:10–07:28:08 · 34 张图 · [打开中英对照稿](24-fabian-hedin.md)

<a name="talk-25"></a>

### 25 · How to build an agent that builds the culture

**Zach Bruggeman** · Ramp · Principal Software Engineer

负责 Ramp 的内部编码 Agent Inspect。

Ramp 让全公司用同一个 Inspect。工程师能看到同事用过的上下文、工具、前后截图和验证记录，也能把好用的工作流补回同一个 Agent。Zach 用一次多人排障和 Review Buddy 说明这个循环。

- [07:30:12](25-zach-bruggeman.md#section-1) Inspect 的使用规模及团队推广时遇到的问题
- [07:32:13](25-zach-bruggeman.md#section-2) 设置成本、信息孤岛和公司共享 Agent
- [07:35:29](25-zach-bruggeman.md#section-3) 如何让每次修改留下可核验的过程
- [07:39:18](25-zach-bruggeman.md#section-4) 公开协作的排障案例与 Review Buddy

录屏 07:30:04–07:44:08 · 40 张图 · [打开中英对照稿](25-zach-bruggeman.md)

[Ramp 工程博客介绍 Inspect](<https://builders.ramp.com/post/why-we-built-our-background-agent>)

<a name="talk-26"></a>

### 26 · Software Factories: Escape from Trash Mountain

**Steve Yegge** · Independent · Independent Advisor &amp; Creator of Beads &amp; Gas Town

Beads 和 Gas Town 创建者，曾在 Google 和 Amazon 从事工程工作。

Steve 用自己迭代多个编排器的经历说明，把 Agent 数量加上去以后，真正费力的是管理工作。任务、token、上下文、团队协作和信任都会影响软件工厂能不能持续运行。

- [07:47:59](26-steve-yegge.md#section-1) 从编排器的迭代史讲到 Gas Town 之后的尝试
- [07:52:50](26-steve-yegge.md#section-2) 不同的 Agent 组织方式与工作管理
- [07:56:06](26-steve-yegge.md#section-3) token 预算、上下文和协作成本
- [08:02:34](26-steve-yegge.md#section-4) 模型的工作条件、信任及对下一年的判断

录屏 07:46:35–08:07:46 · 16 张图 · [打开中英对照稿](26-steve-yegge.md)

[Gas Town 开源项目](<https://github.com/gastownhall/gastown>)

<a name="talk-27"></a>

### 27 · 2026 in LLMs

**Simon Willison** · Independent · Creator of Datasette

Datasette 与 LLM 工具作者，也是 Django 的共同创建者。

Simon 用可现场看到的例子回顾一年内的三个变化：编码 Agent 开始能做实际开发，强模型能在给定目标和工具后长时间搜索解法，生成的游戏也开始有可玩性。适合先建立对过去一年变化的整体印象。

- [08:11:27](27-simon-willison.md#section-1) 编码 Agent 的早期拐点与骑车鹈鹕测试
- [08:14:47](27-simon-willison.md#section-2) 模型变化、工具使用及安全事件
- [08:18:58](27-simon-willison.md#section-3) 更强模型如何在给定目标和工具后完成长任务
- [08:24:55](27-simon-willison.md#section-4) 游戏案例、开发者角色与年初预测回顾

录屏 08:11:12–08:30:28 · 45 张图 · [打开中英对照稿](27-simon-willison.md)

[个人博客与开源作品](<https://simonwillison.net/about/>)
