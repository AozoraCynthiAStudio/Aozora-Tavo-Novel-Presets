# Changelog

## 1.0.4（待发布）

- **尝试修正房号与空间关系理解：** 优先遵循人物卡、世界书、当前场景及前文明确的布局；仅在编号规则已知时才从房号推断楼层。明确区分同层、不同楼层、相邻房间与垂直对应关系，避免把304/305/306误判为不同楼层，或仅凭数字断定房间正上方/隔壁。
- 若编号规则或布局不明，避免武断推断，改用不超出已知事实的中性表述；不强行将常见三位房号规则套用于所有世界观。
- 补充“动作、身体接触、角色反应与关系变化分离”的原则，避免仅因玩家发起或完成接触，就默认 NPC 愿意接受、主动回应或关系自动升级。
- **修正设定执行与文风同质化风险：** 明确人物卡、世界书、对话示例及作者指定文风是实际演绎依据；具体攻略阶段、触发条件与角色变化优先于通用关系发展指导。
- 强调角色变化按设定的范围和程度呈现，未被改变的性格、语言、习惯与价值观继续保留；避免所有角色套用相同的情绪和动作表达。
- 明确亲密场景仍须遵循人物卡与世界书指定的叙述风格，不因场景类型自动切换成通用表达。
- 本次仅调整两份预设已有模块，不新增独立规则层；实际效果仍取决于模型与上下文。

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