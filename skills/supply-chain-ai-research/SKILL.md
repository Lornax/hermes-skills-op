---
name: supply-chain-ai-research
version: 1.0
description: >
  供应链 AI 行业深度研究框架。基于横纵分析法方法论，适配供应链+AI交叉领域。
  触发词：研究、行业分析、竞品分析、深度研究、supply chain、供应链、专题报告
---

# 供应链 AI 深度研究框架

基于横纵分析法（Horizontal-Vertical Analysis）方法论，针对供应链+AI交叉领域定制。

## 数据来源（多源交叉）

  快速通道（基础素材）
  -- aihot.virxact.com：每日 AI 热点精选，覆盖模型/产品/行业/论文/技巧
  -- Brave Search：按关键词搜索中英文新闻（主搜索引擎，免费 2K/月）

  深度搜索（补充+扩展）
  -- arXiv：学术论文（供应链优化、需求预测、物流AI等）
  -- RSS/博客源：行业垂直站点（后续可配 blogwatcher）
  -- 用户指定的其他来源

  专题研究（深度素材）
  -- 本框架的横纵分析法定向搜索
  -- 微信公众号内容（后续接入）

  最终产出：多源交叉验证、去重、整合后的内容精华

## 研究结构

### 纵轴：时间线分析
追踪研究对象从诞生到当下的完整演变，以叙事方式呈现：
- 起源与背景（为什么出现、解决什么问题）
- 关键里程碑（按时间线）
- 技术演进路径
- 市场格局变化
- 当下状态与趋势

### 横轴：同期对比分析
在当前时间截面上与竞品/同类进行系统性对比：
- 核心产品/方案对比（功能、技术路线、商业模式）
- 市场定位与目标客户差异
- 优势与短板
- 融资/规模/团队背景
- 生态与合作伙伴

### 横纵交汇：洞察产出
两条线交叉产生的独到判断：
- 历史如何塑造了当前的竞争位置
- 优劣势的深层根源（非表面现象）
- 未来三种剧本（乐观/基准/悲观）
- 对用户的行动建议

## 输出规格

### 行业监控（周期性）
- 存放：hmWorkspace/content/industry-watch/YYYY-MM/
- 篇幅：2000-4000 字
- 结构：本周核心变化 → 技术动态 → 公司动态 → 政策法规 → 值得关注
- 去重：与 aihot 精选交叉验证，不重复搬运

### 深度研究报告（专题性）
- 存放：hmWorkspace/content/research/YYYY-QX/
- 篇幅：5000-15000 字
- 结构：完整的横纵分析 + 交汇洞察 + 参考资料
- 每份报告含 references/ 子目录存放原始素材链接

### 微信发文素材（待定义格式）
- 存放：hmWorkspace/content/wechat/drafts/
- 格式：待用户后续定义

## 执行流程

1. 明确研究范围（产品/公司/技术/趋势）
2. 多源并行收集信息（aihot + Brave Search + arXiv 等）
3. 交叉验证、去重
4. 纵轴分析（时间线叙事）
5. 横轴分析（竞品对比）
6. 交汇洞察（判断与建议）
7. 生成 Markdown 报告，存入对应目录
8. 更新对应 _index.md 索引

## 注意事项
- 不照搬任何单一数据源，必须多源交叉
- 区分事实与判断，判断需标注依据
- 中文为主，英文源需翻译后融入
- 保持客观，不做广告性质的分析
- 详细数据源策略见 `references/data-sources.md`
- 从业者洞察（算法落地三重墙、AI vs 运筹拆解框架、短链路创新方向、翻译层+反馈闭环）见 `references/ai-embedding-supply-chain-insights.md`
- Logos 产品全景知识库（V1-V4愿景、PRD要点、AI原生性分析、A2A伦理框架）见 `references/logos-product-synthesis.md`。当用户聊到供应链平台产品方向、Logos、车型优化、思考记录器、AI代理人时加载此文件。
- Amazon Connect Decisions 竞品档案（AWS 2026-04 GA，方向与Logos高度重合的最强竞品）见 `references/amazon-connect-decisions-competitor.md`。当用户聊到竞品对比、Amazon供应链、AI Teammate、Adaptive Intelligence时加载此文件。完整分析存于 `hmWorkspace/content/products/supply-chain/2026-05-15-amazon-connect-decisions-analysis.md`。

## 定时任务

- 任务名：supply-chain-ai-weekly（供应链AI周报）
- Cron Job ID：（在 config.local.md 中配置）
- 调度：每周三 12:00
- 覆盖范围：上周三 07:00 ~ 本周三 07:00
- 推送：本地文档 + 微信精简版
- 数据源：智谱MCP（中文🤖）+ Brave（英文🌊）+ RSS（📡）
- 格式：5板块×3条=15条 + 云青洞察
- 关联技能：supply-chain-ai-research, ima-skill
- fallback 模型：（在 config.yaml 中配置 fallback_providers）
- 详细数据源策略：见 `references/data-sources.md`

### 内容范围

物流行业整体动态 + AI 在物流中的应用，越广越好。AI 相关优先级最高，排在前面。
覆盖：仓储自动化、无人驾驶货运、供应链可视化、物流SaaS、港口/海关/冷链/快递、运价指数、政策法规等。

### 分类板块（5个，每板块3条，共15条）

1. 🤖 AI 技术应用 — AI在供应链/物流中的落地案例
2. 🏭 仓储与自动化 — 仓库自动化、机器人、WMS
3. 🚛 运输与无人驾驶 — 自动驾驶货运、车队管理、航运
4. 📊 行业数据与趋势 — 市场报告、融资、指数
5. 🔍 值得关注 — 跨界动态、政策、峰会

### 尾巴

和 AI 日报一样加「💡 云青的洞察」：3-5条趋势判断+行动建议，站在供应链从业者的视角。

### 推送规则

- 本地落库：`hmWorkspace/content/industry-watch/YYYY-MM/YYYY-MM-DD.md`（完整版含链接）
- IMA：推送到「传统物流」笔记本（完整版含链接）
- 微信：精简版，格式同 AI 日报（标题+2-3句摘要，不放链接，表情+加粗排版，🔥aihot / 🌊Brave 标记）
- 数据源标记同 AI 日报规则（见 hmworkspace-conventions skill）
