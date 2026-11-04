# Changelog

## 1.0.6（2026-11-04）

- **修复玩家心理素材被正文接续规则遗漏的情况：** 两份预设均明确将玩家本轮已写出的心理活动、感受、猜测、主观判断与打算纳入小说正文素材，不再只强调台词与外在动作。
- 保持想法、猜测、意图与客观事实、实际行动之间的区别；未说出口的心理不自动成为 NPC 的知情信息，也不擅自编造玩家未提供的新心理或决定。
- 正文从玩家本轮素材自然开始，允许依据内容分成连续的开头段落，保留原有顺序及只呈现一次的原则，不机械挤在第一段。
- 只改动原有正文接续提示词，不新增槽位，不触及关系、文风、世界或其他功能规则。这是提示词层面的修正，实际表现仍需模型测试。

## 1.0.5（2026-11-04）

- 调整两份预设对玩家已明确写入剧情的行为与结果的处理方式，尝试减少过度审查、过严判断或无依据地跳过已发生事件的情况。
- 保持角色对事件的反应由人物卡、世界书、既有关系和当前情境决定，不把反应与事件是否发生混为一谈。
- 保留原有提示词槽位、启用状态和导入结构；这是提示词层面的尝试，实际表现可能因模型和上下文而异。

## 1.0.4（2026-10-30）

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