# 供应链AI周报 — 数据源策略

## 数据源分工

### 中文源（智谱 MCP zai_web_search）🤖

搜索关键词（每次必搜）：
- "物流 AI" + 过去一周
- "供应链 人工智能" + 过去一周
- "仓储自动化" + 过去一周
- "无人驾驶 物流" + 过去一周
- "物流SaaS" + 过去一周

可选关键词（轮换使用）：
- "冷链 物流"
- "港口 智慧"
- "快递 科技"
- "运价 指数"
- "供应链 数字化"

中文垂直网站（通过 Brave 或智谱 MCP 搜索时覆盖）：
- 罗戈网/物流沙龙（logclub.com）— 国内物流人社区，偏实操
- 物流指闻/运联智库 — 国内物流行业活跃媒体
- 36氪/虎嗅 "物流" 标签 — 中文 AI+物流 报道

### 英文源（Brave Search）🌊

搜索关键词（每次必搜）：
- supply chain AI news
- logistics automation news
- warehouse robotics
- autonomous trucking
- supply chain visibility platform

可选关键词（轮换使用）：
- freight market trends
- last mile delivery innovation
- cold chain logistics technology
- port automation
- supply chain resilience

### RSS 源（blogwatcher）📡

优先级高（每周必采）：
1. FreightWaves (freightwaves.com/feed)
2. Supply Chain Dive (supplychaindive.com/rss)
3. Logistics Viewpoints (logisticsviewpoints.com/feed)

优先级中（轮换采集）：
4. Transport Topics (ttnews.com/rss)
5. Highways Today (highwaystoday.com/feed)
6. Automation World (automationworld.com/feed)

优先级低（月度深度）：
7. McKinsey Supply Chain (mckinsey.com/features/ supply-chain)
8. Gartner Supply Chain (gartner.com/en/supply-chain)

### 学术源（arXiv）

搜索关键词：
- supply chain optimization
- logistics deep learning
- demand forecasting neural
- vehicle routing problem
- inventory management reinforcement learning

## 数据源标记规则

- 🔥 aihot 精选（快速通道）
- 🌊 Brave Search（英文主搜）
- 🤖 智谱 MCP（中文主搜）
- 📡 RSS/blogwatcher（订阅源）
- 📄 arXiv（学术论文）

## 去重规则

1. 同一事件多源报 → 取信息最完整的版本，标注所有来源
2. 中英文同一事件 → 中文版为主（用户阅读偏好），英文补充细节
3. RSS 和 Brave 搜索重复 → 优先 RSS（时效性更可控）

## 质量控制

- 每条新闻必须有明确来源和日期
- 不确定的信息标注"待验证"
- AI相关内容优先级最高，排在板块前面
- 物流行业整体动态其次
- 纯广告/软文不收录
