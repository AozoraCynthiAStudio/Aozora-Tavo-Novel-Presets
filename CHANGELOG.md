# Changelog

## 1.0.4（待发布）

- **尝试修正房号与楼层关系理解：** 明确区分楼栋、单元、楼层和房间编号；对于常见三位房号示例，304/305/306属于三楼，403属于四楼。若作品未明确编号规则，则不武断推断楼上、楼下或相邻关系。
- 本次仅扩展两份预设已有的空间连续性提示，不新增独立规则层；实际效果仍取决于模型与上下文。

## 1.0.3

- **尝试修复部分相对时间表达的理解：** 明确“今天、明天、后天”等词语应以故事当前日期为参照，并让已建立的约定和计划保留固定目标时间，避免剧情推进后仍反复把同一事件称为“明天”。
- 强调虚构故事时间应依据场景标记、用户指定的时间跳跃和已发生的剧情变化，不应直接套用现实日期，也不应仅因多生成一轮就默认过了一天。
- This is a prompt-level attempt; results may vary across models and context.

## 1.0.2

- **2026-10-25 · Updated release package:** Clarified Eveline's adult-narrative guidance to distinguish private adult thoughts/actions from interactions between characters, without changing the prompt structure. Iveya is unchanged.

- Clarified Eveline's high-level living-chronicler identity in the existing Eveline core prompt, without adding prompt slots or changing their enabled states.

First public repository baseline.

- Refined scene writing to better integrate spatial composition, physical behavior, gaze, expression, voice, pauses, and relevant environmental details.
- Emphasized continuous character presence throughout a scene, rather than relying mainly on dialogue with isolated gestures.
- Preserved the goal of incorporating the player's latest in-story words and actions into the prose.
- Retained narrative continuity, character logic, viewpoint boundaries, and natural scene extension.
- Avoided a fixed minimum response length; the goal is sufficient descriptive depth rather than length for its own sake.
- Kept two distinct preset approaches:
  - **Iveya Zhiyu:** default-style prompt-slot organization, without a standalone narrative persona.
  - **Eveline Zhijing:** custom layered prompt structure, an independent narrative identity, and adult-intimacy guidance.

Results may vary across models, API providers, character cards, world information, and generation settings.