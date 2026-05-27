# aihot

AI HOT (aihot.virxact.com) 中文 AI 资讯查询 Skill。

调用公开 API，无需 API Key。支持：
- 每日 AI 日报（5 大板块）
- 精选动态（默认）/ 全量动态
- 按分类筛选（模型/产品/行业/论文/技巧）
- 关键词搜索
- 时间窗口筛选

## 文件说明

```
aihot/
├── SKILL.md           # 主技能文档（含完整 API 用法和输出格式）
└── templates/
    └── wechat-daily.md  # 微信推送格式模板
```

## 快速开始

```bash
# 装到 Hermes skills 目录
cp -r aihot ~/.hermes/skills/media/aihot
```

装完后，在 Hermes 中说"AI 日报"或"今天 AI 圈有什么"即可触发。

## 数据源

- aihot.virxact.com — 公开匿名 API，600 req/min/IP 限流
- 可配合 Brave Search 做中英文交叉验证
