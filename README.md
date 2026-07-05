# hermes-skills-op

Hermes Agent 的开源技能包。每个 skill 都是一个独立的 SKILL.md + 可选的 references/templates，可以直接装到 [Hermes Agent](https://github.com/nousresearch/hermes-agent) 中使用。

## 技能列表

| 技能 | 说明 | 类别 |
|------|------|------|
| [aihot](skills/aihot/) | AI HOT 中文 AI 资讯查询。调用 aihot.virxact.com 公开 API，获取每日 AI 日报、精选动态、模型发布、产品更新等。无需 API Key。 | 媒体 |
| [diary-manager](skills/diary-manager/) | 日记管理技能。随手记碎片，自动提炼、记账、同步多主线 tracker（花销/学习/生活/文化/亲密关系/待办）。支持 Tracker 交叉检查、周/月总结、月度成长剖析（乔哈里视窗）、语音转文字处理、饮食卡路里估算、健康数据集成。v3.2。 | 效率 |
| [supply-chain-ai-research](skills/supply-chain-ai-research/) | 供应链 AI 行业深度研究框架。基于横纵分析法，支持多源数据交叉验证、周报自动生成。 | 领域 |

## 怎么用

把整个 skill 文件夹复制到你的 Hermes skills 目录下即可：

```bash
# Hermes skills 目录通常在：
cp -r skills/aihot ~/.hermes/skills/media/aihot
cp -r skills/diary-manager ~/.hermes/skills/productivity/diary-manager
cp -r skills/supply-chain-ai-research ~/.hermes/skills/domain/supply-chain-ai-research
```

或者只复制单个 SKILL.md 到对应位置。

## 关于个人配置

部分 skill（如 diary-manager）需要 `config.local.md` 来配置个人专属信息（名字、路径、时区等）。SKILL.md 中所有 `{{占位符}}` 从 config.local.md 读取。

这样做是为了：
- SKILL.md 保持通用，可以开源分享
- 个人隐私数据隔离在 config.local.md（不上传 GitHub）

## 贡献

欢迎提 issue 和 PR。如果你基于这些 skill 改出了更好用的版本，也欢迎分享。

## License

MIT
