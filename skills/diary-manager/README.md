# diary-manager

Hermes Agent 日记管理技能（通用版）。

随手记碎片，自动提炼、记账、同步多主线 tracker。支持：
- 每日日记写入 + 智能提取（TODO/灵感/行业观察）
- 多主线 tracker 同步（花销/学习/生活/文化/待办）
- 每日自动提炼 cron（像朋友写的一段话，不是流水账）
- 周/月总结
- 月度成长剖析（乔哈里视窗双视角互评）
- 面试记录处理
- 每日记账（只记用户明确说的花销）

## 文件说明

```
diary-manager/
├── SKILL.md                              # 主技能文档（通用版，所有个人数据通过 {{占位符}} 隔离）
├── references/
│   └── vision-model-pricing-research.md  # 视觉模型价格对比参考
└── templates/
    ├── daily-entry.md                    # 每日日记模板
    └── growth-profile.md                 # 月度成长剖析模板（乔哈里视窗）
```

## 需要配置

使用前需要创建 `config.local.md`（与 SKILL.md 同目录），配置：

```markdown
# 个人配置

- 用户称呼：你的名字
- 代理名称：你的AI助手名字
- 日记根目录：/path/to/diary/
- Tracker 目录：/path/to/tracker/
- Growth 目录：/path/to/growth/
- 系统时区：你的系统时区（如 America/Los_Angeles）
- 用户时区：你的所在地时区（如 Asia/Shanghai）
- 天气城市：你的城市
```

SKILL.md 中所有 `{{占位符}}` 会从这个文件读取。这样做是为了个人隐私数据不进入版本控制。

## 安装

```bash
cp -r diary-manager ~/.hermes/skills/productivity/diary-manager
# 然后创建 config.local.md
```
