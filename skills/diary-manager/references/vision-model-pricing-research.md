# 视觉模型价格调研（2026-05-25）

> 如视觉能力到期需切换，此文档记录各平台对比。

## 各平台视觉模型对比

### 智谱（Zhipu/GLM）
- 用户有 Coding Plan，但**视觉模型不在套餐内**，需单独按量付费
- GLM-4V-Flash：公开页面标注免费，但 Coding Plan 用户需确认是否适用
- GLM-4.6V：输入 ¥1/百万tokens，输出 ¥3/百万tokens（性价比最高的付费模型）
- **结论**：Coding Plan 不含视觉模型，不能直接用免费额度的视觉模型

### 百炼（阿里云 DashScope）
- qwen-vl-plus：输入 ¥0.0015/千tokens，输出 ¥0.006/千tokens（最便宜）
- qwen-vl-max：输入 ¥0.003/千tokens，输出 ¥0.012/千tokens
- qwen3-vl-flash：阶梯计费，性价比高
- **用户意向**：到期后可能转百炼普通套餐继续用，不走 Coding Plan

### 月之暗面（Kimi/Moonshot）
- moonshot-v1-8k-vision：¥12/百万tokens（统一价）
- 新用户送 ¥15 额度，500次/月可用免费额度覆盖

### MiniMax
- MiniMax-VL-01：输入 ¥1/百万tokens，输出 ¥8/百万tokens
- M2.5 系列：图像理解按次数扣（每次=3次请求）

## 待用户确认
- 用户说6月2号前会自己对比各平台图像识别质量后给结论
- 届时根据用户选择切换 config.yaml 中的 auxiliary.vision 配置

## 调研教训
- ⚠️ 不能只看官方定价页面的"免费"标签就下结论，必须确认该模型是否在用户当前套餐/plan内
- ⚠️ Coding Plan 是编码专用套餐，视觉模型、语音模型等通常不在套餐范围内
