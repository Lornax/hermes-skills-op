# 日记管理技能 · 个人配置模板
# 复制此文件为 config.local.md 并填写你的信息。
# cp config.local.example.md config.local.md

## 用户信息

- 用户称呼：你的昵称
- 用户真名：你的真名（可选）
- 代理名称：你的 AI 助手名字

## 时区配置

- 系统时区：PDT（UTC-7）  # 你的电脑/服务器运行的时区
- 用户所在地时区：Asia/Shanghai（UTC+8）  # 你实际所在的时区
- 时差：15小时  # 用户时区 - 系统时区的差值（小时）
- 时区转换命令：TZ=Asia/Shanghai date '+%Y-%m-%d %H:%M'  # 获取用户时间的命令

## 路径配置

- 日记根目录：/Users/YOUR_USERNAME/diary/
- Tracker 目录：/Users/YOUR_USERNAME/diary/tracker/
- Growth 目录：/Users/YOUR_USERNAME/content/growth/
- 天气城市：Beijing  # wttr.in 支持的城市名

## Cron 任务（在 Hermes 中创建后填入 Job ID）

- 每日提炼 Job ID：YOUR_DAILY_JOB_ID
- 每日提炼调度：15 18 * * *  # 系统时区的 cron 表达式
- 周总结 Job ID：YOUR_WEEKLY_JOB_ID
- 周总结调度：0 20 * * 0
- 月总结 Job ID：YOUR_MONTHLY_JOB_ID
- 月总结调度：0 20 1 * *
- 月度成长剖析 Job ID：YOUR_GROWTH_JOB_ID
- 月度成长剖析调度：0 5 24 * *  # 每月24日

## 模型配置（可选）

- 主模型：你的默认模型
- 降级模型：备用模型（限频时切换）

## 个人偏好（可选）

- 消费态度：适度劝省 / 不干预 / 鼓励消费
- 医疗建议：不给具体用药建议 / 允许一般建议
- 日记提炼格式：自然段叙述式 / 自定义
- 时间格式：24小时制 / 12小时制
