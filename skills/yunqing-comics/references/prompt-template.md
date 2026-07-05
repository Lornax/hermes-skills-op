# 生图提示词模板

每张图单独生成。根据正文内容替换变量，不要把多张图拼在一张里。

```text
Use case: illustration-story
Asset type: Chinese article body illustration in the Yunqing Comics recurring IP style
Primary request: Create one standalone hand-drawn article illustration that explains this idea: {核心意思}
Scene/backdrop: clean warm white paper background with generous empty space; only a few simple desk/story objects if needed
Subject: recurring original IP characters, a small fluffy cloud and a tiny clear bottle. The cloud is {云朵动作}; the bottle is {瓶子动作}. They must perform the core conceptual action, not decorate the scene.
Structure type: {前后对比 / 系统局部 / 输入处理输出 / 方法分层 / 角色状态 / 概念隐喻}
Composition/framing: {具体构图：主物件、左右/前后关系、信息如何移动}
Style/medium: cute independent hand-drawn cartoon IP, loose pencil and fine ink linework, slightly wobbly imperfect outlines, soft watercolor wash accents, simple black dot faces, warm but not childish, polished article illustration
Color palette: warm off-white, graphite gray lines, pale sky blue, transparent soft blue, muted peach, cream yellow, tiny honey-yellow star details
Materials/textures: light paper grain, soft pencil texture, translucent bottle wash, simple rounded handmade shapes
Text: {默认 no readable text；如需要，列出 1-5 个极短标注}
Constraints: one image explains only one core idea; keep the characters central to the action; preserve generous white space; use a fresh physical metaphor for this article
Avoid: avoid photorealism, 3D render, hard vector logo style, PPT infographic look, dense UI screenshot, complex architecture diagram, lots of text, branded elements, copying Xiaohei or any reference character
```

## 让角色更参与

如果角色变成装饰，用这个方向重写：

```text
Regenerate with the same core idea, but make the cloud and bottle perform the conceptual work. The cloud should physically move, connect, soften, or gather the messy part. The bottle should record, store, filter, validate, or protect the organized result. If the characters are removed, the metaphor should no longer work.
```

## 减少信息图感

```text
Regenerate as a warm hand-drawn article illustration, not a diagram. Remove title bars, grid layout, formal nodes, excessive arrows, and explanatory labels. Keep one main handmade object and one clear action.
```
