# yunqing-comics

云青漫画是一个中文文章正文插图 Skill。它用固定的原创 IP 角色「小云朵」和「小瓶子」，把文章里的抽象观点、流程、结构、状态或隐喻，转成温暖、克制、可解释的手绘漫画配图。

它不是通用贴纸生成器，也不是 PPT 信息图生成器。它更像一个文章旁边的解释草图助手，先理解内容，再把一个认知动作画出来。

## 支持场景

- 给中文公众号文章规划正文配图
- 把方法论、AI 工作流、产品思考画成低科技物理隐喻
- 输出 shot list、单张生图提示词和迭代建议
- 检查图像是否符合云青漫画风格

## 文件说明

```text
yunqing-comics/
├── SKILL.md
├── agents/
│   └── openai.yaml
├── assets/
│   └── examples/
└── references/
    ├── characters.md
    ├── composition-patterns.md
    ├── prompt-template.md
    ├── qa-checklist.md
    └── style-dna.md
```

## 安装

```bash
cp -r skills/yunqing-comics ~/.hermes/skills/creative/yunqing-comics
```

装完后，可以这样调用：

```text
Use $yunqing-comics to turn this Chinese article section into a Yunqing cloud-and-bottle hand-drawn illustration.
```

## 设计原则

- 一张图只解释一个核心动作、结构、状态或隐喻
- 小云朵和小瓶子必须参与核心动作，不能只是站在旁边卖萌
- 默认温暖白底、手绘细线、轻水彩、大量留白
- 少文字，少箭头，少结构图感
- 每篇文章重新发明隐喻，不复刻参考图、已有示例或他人 IP

## 致谢

云青漫画 Skill 最早受到 Ian 的 [helloianneo/ian-xiaohei-illustrations](https://github.com/helloianneo/ian-xiaohei-illustrations) 启发。这个「中文小黑怪诞正文配图生成 Skill」曾冲到 GitHub 周榜第 2，让我意识到，一个好 Skill 不只是把 prompt 写长，而是把审美判断、任务边界、工作流和质量检查沉淀成可复用的协作方式。

在这个基础上，云青漫画做了自己的延展，加入了小云朵和小瓶子的原创角色分工、中文文章正文插图场景、低科技物理隐喻生成法，以及面向「可爱但有解释力」的 QA 规则。

特别感谢 Ian 和小黑配图 Skill 带来的启发。云青漫画不会复刻小黑 IP、黑豆角色或参考构图，也请使用者尊重原创边界。
