<div align="center">

# Aozora · Tavo Novel Presets

**双生小说式描写预设 · Two Novel-Style Writing Presets for Tavo**

面向互动小说与角色扮演的两种叙事预设：共享小说式描写的基础目标，但在提示词结构与叙事身份上采用不同路线。

Two narrative presets for interactive fiction and roleplay. They share a novel-style writing foundation, while taking different approaches to prompt structure and narrative identity.

[![Version](https://img.shields.io/badge/version-1.0.2-5277C3?style=flat-square)](https://github.com/AozoraCynthiAStudio/Aozora-Tavo-Novel-Presets/releases)
[![License: MIT](https://img.shields.io/badge/License-MIT-2EA44F?style=flat-square)](LICENSE)
[![Language](https://img.shields.io/badge/language-中文%20%2F%20English-8A63D2?style=flat-square)](#language)

**[前往 Releases 获取正式版本 · Get the published release](https://github.com/AozoraCynthiAStudio/Aozora-Tavo-Novel-Presets/releases)**

</div>

---

## 中文

## 项目定位

Aozora · Tavo Novel Presets 是一组为 Tavo 互动小说体验设计的社区预设。我们关注的不只是“角色下一句说什么”，也包括玩家本轮提供的言行如何进入小说正文、人物如何通过动作与细节呈现、剧情如何在不偏离玩家意图的前提下自然延续。

两份预设的共同方向是：

- **把玩家本轮的戏内输入写进小说。** 对话、动作和已明确的剧情事实应自然进入正文开头，再衔接角色回应；不是只让 NPC 听见或复述玩家的话。
- **重视剧情连续性。** 旧回合是已经发生的历史，不是每轮都要重写的草稿。保留人物状态、关系变化、物件、地点、承诺与未解决事件，避免无必要的回顾和重复。
- **让场景更有层次。** 对话之外，还可以描写空间关系、身体动作、眼神、表情、声音、停顿、环境，以及这些细节如何改变当下互动。
- **尊重人物与世界设定。** 角色依据自己的性格、经历和知情范围行动；世界可以自然运转，但不能为了“主动”而覆盖玩家已经确定的剧情方向。
- **按场景决定篇幅。** 重要互动可以充分展开，日常场景也可以保持轻松、平静或简短。不设固定最低字数，不为了显得文学化而灌水，也不要求每轮都发生重大变化。

这是一套写作风格与叙事组织方面的指导，不是模型、采样参数或 Tavo 引擎的修改。实际表现取决于所用模型、API 服务、人物卡、世界书、历史长度与生成设置。

## 两份预设的区别

| | **伊薇娅·织语** | **伊芙琳·织境** |
|---|---|---|
| 核心路线 | 沿用 Tavo 默认风格的提示词槽位组织 | 在 Tavo 原有槽位上增加分层叙事指导 |
| 叙事身份 | 不额外设立独立叙事人格 | 具有独立的后台叙事身份 Eveline |
| 主要重点 | 小说式接续、连续性、场景表现与通用适配目标 | 在共同写作基础上，更明确地组织人物主动性、世界反馈、细节表现与成年角色亲密叙事 |
| 结构取向 | 简洁、接近常规预设结构 | 模块更细、规则更明确 |
| 更适合 | 希望使用中性、通用的小说式描写，不希望额外叠加人格设定的玩家 | 希望使用有明确叙事身份和更细分规则的玩家，尤其关注关系发展、世界自主性与成年角色亲密互动描写的玩家 |

两份预设不是基础版与高级版，也不代表某一份在所有模型上都更好。伊芙琳的规则更多、身份更鲜明，不等于它必然写得更好或更长；伊薇娅结构相对简洁，也不代表它缺少小说式描写能力。

---

## 伊薇娅·织语

### 一句话定位

**不额外设立叙事人格，以相对简洁的提示词结构，专注于小说正文、剧情连续性与场景表现。**

### 结构是什么样的？

伊薇娅沿用 Tavo 常见的提示词槽位与组织方式。配置保留人物描述、人物性格、用户 Persona、Scenario、世界书前后置内容、对话示例和聊天历史等原有上下文入口；核心写作要求集中在主提示词中，不额外加入一个会在故事里拥有独立身份的叙事角色。

配置中也保留了原有的可选槽位；部分辅助扩写、辅助提示与历史后置指令默认关闭或留空，避免不必要的额外规则叠加。

### 它具体做了什么？

**1. 把玩家输入转成小说正文**

当玩家本轮给出戏内对白、动作或剧情事实时，要求正文开头先将这些内容自然写成小说语言。可以润色措辞、节奏和即时感官细节，但应保留玩家原本的意思、行动顺序、视角和结果。不能只让 NPC 听见玩家的话，再由 NPC 转述一遍来代替正文呈现。

如果玩家只发出戏外指令，或只是要求继续而没有新的戏内动作，则不虚构玩家行为。

**2. 把历史当作历史，而不是重复素材**

已完成的前文用于理解当前状态，不应每轮重新演一遍或变成剧情摘要。只有当过去的事件确实影响当前互动，才自然地简短提及；明确要求回顾、闪回或重写时除外。

**3. 让人物关系随实际经历变化**

人物关系不被固定标签锁死。通过已经发生的互动、信任、疏远、承诺和冲突表现关系变化；不凭空加速，也不因每轮重新生成就把已有熟悉感清零。若人物卡或世界书定义了关系数值，按其明确含义理解，不自行编造数值阈值。

**4. 不把场景限制在一句回应里**

NPC 可以在符合性格和情境时主动回应，场景也可以自然延续到相关动作、环境反馈或情绪余波。但不要求每轮强行制造新事件、换地点或推动关系升级。玩家明确指定的方向优先。

**5. 增强画面感与细节层次**

在相关时刻描写人物所处的位置、彼此距离、身体姿态、手部动作、眼神、表情、说话节奏、停顿和环境细节。动作要有合理的过程与反馈，细节要服务人物和情境，而不是给每句话机械附加一个动作。

**6. 保留自然篇幅与视角边界**

重要场景可以写得细致，普通日常可以保持轻盈。不设固定字数目标，也不强制使用第一人称；沿用故事实际建立的叙述视角，并遵守该视角能感知的信息范围。

### 适用场景

- 希望改善玩家输入与小说正文之间的衔接，让聊天记录读起来更像连续的小说。
- 希望加强动作、眼神、表情、空间和环境细节，而不只依靠对白推进。
- 希望剧情连续，但不希望预设每轮都主动扩写很多或替玩家决定剧情走向。
- 希望提示词结构接近 Tavo 常规槽位，不想额外加入独立叙事人格。
- 希望先从相对中性的版本开始，根据自己使用的模型和人物卡调整。

伊薇娅的目标是尽量保持通用、简洁的结构；这是一种设计取向，不代表已经实测兼容所有模型或 API 服务。

---

## 伊芙琳·织境

### 一句话定位

**以 Eveline 作为后台叙事身份，在 Tavo 原有上下文槽位之外，用多个职责清晰的规则层组织人物、世界、连续性与描写方式。**

### Eveline 是什么身份？

伊芙琳不是默认会走进故事、自我介绍或与 NPC 抢戏的剧情角色。她是预设中用于组织叙事工作的**后台叙事身份**：帮助模型理解本轮输入、人物关系、历史事实、世界反馈和表现要求，再把这些要求落实为小说正文。

除非玩家明确选择与 Eveline 本人互动，否则规则要求她不要在故事正文里解释自身身份、展示后台规则或取代当前角色成为场景中心。

因此，伊芙琳与伊薇娅的关键差异不只是规则数量，还在于：伊芙琳具有明确的叙事身份，并将写作指导拆成多个相互配合的模块。

### 结构是什么样的？

伊芙琳在 Tavo 原有的人物、Persona、Scenario、世界书、对话示例和聊天历史等槽位前后，加入了多个职责分明的叙事规则层。当前配置共有 22 个提示词条目，其中包含原有上下文槽位、主提示词、继续与输出格式指令，以及默认关闭或留空的辅助槽位。

主要自定义规则层包括：

| 规则层 | 负责什么 |
|---|---|
| **用户身份** | 以当前 Tavo 的用户角色为准，不因预设中的称呼擅自给玩家追加身份。 |
| **Eveline 核心** | 区分玩家指令与戏内内容，确定本轮叙事起点、职责和优先级。 |
| **人物、关系与主动性** | 让角色保持自己的性格、关系连续性与行动动机，不套用统一人格模板。 |
| **成年亲密叙事** | 专门指导明确成年虚构角色之间的亲密情感与行为如何保持自然、连续，并尊重当前意愿与边界。 |
| **连续性、记忆与知情边界** | 管理时间、地点、人物状态、物件、关系、承诺与秘密；限制角色只使用自己有理由知道的信息。 |
| **世界、场景与剧情动能** | 让 NPC 与环境在合理范围内拥有自己的目标和反馈，避免场景在一句回应后无故收住，也不强迫剧情升级。 |
| **叙事表现与动态强度** | 根据场景重要性调整细节密度，综合运用空间、动作、眼神、声音、环境与互动反馈。 |
| **空间、身体与时间连续性** | 检查动作过程、身体位置、物件状态和时间推进是否合理；尊重玩家主动跳过的过渡。 |

此外，主提示词与“继续”“最后”等指令共同强调：最新一轮的戏内内容应自然进入小说正文，较早的剧情则作为已经发生的历史；输出应沿用当前故事视角和要求的正文格式，而不是展示规则或分析过程。

### 它的核心理念是什么？

**不是靠一条特别强硬的指令包办所有事情，而是把叙事工作拆开，让不同规则分别负责自己擅长的部分。**

- **身份与职责明确：** Eveline 是叙事操作层，不自动成为剧情中的新角色。
- **人物有自己的逻辑：** 角色可以主动、迟疑、拒绝、亲近或改变节奏，但行为要来自角色设定与实际经历。
- **世界可以自然运转：** NPC 和环境不只是等待玩家提问的静态背景，但其自主性不能覆盖玩家明确指定的剧情。
- **连续性是长期的：** 已经建立的关系、事实与后果应持续影响后续，不因新一轮生成而重置。
- **描写强度动态调整：** 重要场景可以放慢、细写；普通日常不必被强行写成重大转折。
- **亲密叙事关注连续性与边界：** 在模型和服务平台允许的范围内，减少没有情境依据的突然回避；同时尊重新的疑虑、拒绝、不适和边界变化。

### 关于成年亲密叙事规则

伊芙琳包含一层面向**明确成年人的虚构角色**的亲密叙事指导。它主要处理的是写作方式与上下文连续性，例如：

- 不因场景进入暧昧或亲密阶段，就突然把人物关系重置或切换成无关的说明口吻。
- 让角色的情感、动作、回应和节奏符合已有互动及人物性格，而不是机械套用固定阶段。
- 如果相同互动中没有新的疑虑，不必每一步都重复同一种确认流程；但出现新的边界、拒绝、不适、退缩或停止时，应认真回应并调整。
- 不替玩家决定感受或回应，也不以过去的亲密自动推定当前意愿。

需要明确的是：这是一套叙事风格指导，**不是能够解除模型或 API 服务限制的技术模块，也不保证特定内容一定会被生成**。如果模型或服务平台不允许某类内容，预设不能改变这一点。公开介绍应以“成年亲密叙事指导”“减少无必要的回避性表达”等准确描述为主，而不承诺破限效果。

### 适用场景

- 希望使用一个有明确叙事身份、但不会自动闯入剧情的后台写作人格。
- 希望把人物关系、世界自主性、连续性、动作逻辑和场景细节分别组织成明确规则。
- 经常进行较长的互动小说，希望人物、物件、关系和事件后果更稳定地延续。
- 希望 NPC 能在符合性格与上下文时主动行动，而不是每轮只给一句回应。
- 关注成年虚构角色的亲密情感与行为描写，并理解实际表现仍受模型和服务平台限制。
- 能接受更细分的提示词结构，并愿意根据所用模型测试和调整。

如果你更看重简洁的默认槽位结构、尽量减少额外叙事身份，或者使用限制严格的模型与 API 服务，可以先尝试伊薇娅。

---

## 安装、下载与修改

### 获取正式版本

**请从 GitHub Releases 页面获取正式发布版本：**

**[前往 Releases 下载 · Download from Releases](https://github.com/AozoraCynthiAStudio/Aozora-Tavo-Novel-Presets/releases)**

发布版本与源文件分开管理，建议普通玩家优先下载 Release 中标记的正式版本；想研究规则、查看差异或自行修改的玩家，可以直接浏览仓库中的源配置：

- [查看伊薇娅源配置](presets/Iveya-Zhiyu-1.0.2.json)
- [查看伊芙琳源配置](presets/Eveline-Zhijing-1.0.2.json)

### 安装建议

1. 先备份自己当前使用的 Tavo 预设。
2. 从 Releases 选择想体验的预设版本并下载。
3. 在 Tavo 中导入 JSON 文件。
4. 导入后检查提示词槽位、启用状态与顺序是否符合预期。
5. 用熟悉的人物卡、世界书和模型体验几轮，再决定是否调整。

不同 Tavo 版本或导入方式可能存在差异，请以实际界面为准。

## 兼容性与反馈

- 实际表现会受到模型、API 服务、人物卡、世界书、聊天历史长度与生成设置影响。
- 两份预设都不保证固定的回复字数、第一人称叙述或完全一致的文风。
- 伊薇娅以通用和相对简洁为设计目标；这不等于已经验证兼容所有模型或中转服务。
- 伊芙琳包含更明确的叙事身份与分层规则，部分模型可能更能响应，也可能出现规则遵循不稳定或提示词冲突。
- 本项目不修改模型本身，也不绕过服务端限制。
- 欢迎提交可复现的问题与使用反馈。社区反馈会作为后续迭代的参考，但不代表每项建议都会合并进主版本。
- 本项目为独立社区项目，不是 Tavo 官方项目，也不代表 Tavo 或任何模型服务商的官方背书。

## 版本与许可证

当前预设版本：**1.0.2**。

本项目使用 **MIT License**，详情见 [LICENSE](LICENSE)。你可以按许可证条款使用、修改和再发布；分享修改版时，请保留适用的版权和许可证声明。

---

<a id="language"></a>

## English

## Project overview

Aozora · Tavo Novel Presets offers two community presets for interactive fiction and roleplay in Tavo. The shared goal is to turn the player's latest in-story input into natural novel prose, maintain continuity, and portray scenes through more than dialogue alone.

Both presets aim to:

- Render the player's latest in-story dialogue, actions, and established beat at the beginning of the story passage, while preserving their meaning and outcome.
- Treat completed turns as history rather than material to replay every turn.
- Use physical behavior, gaze, expression, voice, pauses, spatial relationships, and relevant environmental details to create a more legible scene.
- Preserve character logic, world information, viewpoint boundaries, and cause-and-effect continuity.
- Let scene length follow the situation rather than a fixed word count or a requirement to escalate every turn.

These are narrative and writing instructions, not changes to the model, sampling parameters, or Tavo engine. Results depend on the model, API provider, character cards, lore, history length, and generation settings.

## Iveya Zhiyu

**A relatively compact, neutral novel-writing preset without a separate narrative persona.**

Iveya follows Tavo's familiar prompt-slot organization. It retains the usual context slots for persona, character description and personality, scenario, lorebook content, dialogue examples, and chat history. The core writing guidance is concentrated in the main prompt rather than spread across a separate narrator identity.

Its main rules are:

1. **Render the latest player beat in prose.** Include the player's supplied in-story words and actions in the opening paragraph, polishing phrasing and immediate texture without changing meaning, order, viewpoint, or outcome.
2. **Preserve completed history.** Use prior turns to understand the present; do not routinely replay or summarize them.
3. **Maintain relationship continuity.** Let familiarity, trust, distance, and conflict reflect established events rather than resetting or advancing them mechanically.
4. **Continue naturally when appropriate.** A scene may extend into relevant reactions, actions, and consequences, without forcing a new event or overriding the player's direction.
5. **Build scene texture.** Use spatial composition, body language, gaze, expression, voice, pauses, and environmental details when they serve the moment.
6. **Respect viewpoint and pacing.** Do not invent the player's choices or private thoughts. There is no fixed minimum word count and no forced first-person viewpoint.

Iveya is intended for players who prefer a more neutral structure, want novel-style prose without an additional narrator persona, or want to start with a relatively compact preset. This is a design goal, not a guarantee of universal model or API compatibility.

## Eveline Zhijing

**A layered writing preset with Eveline as a distinct backstage narrative identity.**

Eveline is not automatically a new character who enters the story, introduces herself, or takes attention away from the cast. She acts as a backstage narrative identity that organizes how the model interprets the latest input, character relationships, continuity, world feedback, and prose requirements. Unless the player explicitly interacts with Eveline, the rules instruct her not to take over the story's foreground.

The current configuration contains 22 prompt entries, combining Tavo's standard context slots with custom layers, a main prompt, continuation/output instructions, and auxiliary slots that are disabled or left empty.

Its eight main custom layers are:

- **User identity:** Follow the current Tavo user role without inventing extra identity details from preset wording.
- **Eveline core:** Separate in-story material from player/author instructions and establish the turn's narrative starting point and priorities.
- **Character, relationships, and initiative:** Preserve character-specific behavior and let relationships evolve through actual events, without forcing stages or generic personalities.
- **Adult intimacy guidance:** For clearly adult fictional characters, maintain emotional and interaction continuity while respecting present willingness and boundaries.
- **Continuity, memory, and knowledge boundaries:** Track relevant locations, possessions, relationships, promises, secrets, and consequences; do not give characters knowledge they could not reasonably have.
- **World, scene, and narrative momentum:** Allow NPCs and the environment to act naturally within the space left open by the player's direction, without forcing escalation.
- **Narrative performance and dynamic intensity:** Adjust descriptive depth to the scene and combine space, physical behavior, gaze, voice, environment, and feedback.
- **Spatial, physical, and temporal continuity:** Keep action sequences, positions, object states, and time progression coherent, while respecting deliberate scene jumps.

Eveline is suited to players who want a distinct narrative identity, more explicit organization of character and world behavior, stronger attention to long-running continuity, and more guidance for adult fictional intimacy where permitted.

### Adult-intimacy guidance and limits

This layer applies to fictional characters who are clearly adults. It aims to keep emotional and physical interactions consistent with established context, avoid unnecessary abrupt evasions, and respond appropriately to new uncertainty, discomfort, refusal, or changing boundaries. It does not decide the player's feelings or responses.

This is writing guidance—not a technical bypass of model or API restrictions—and it cannot guarantee that a specific category of content will be generated. The model and service provider's rules still apply.

## Choosing and installing

- **Choose Iveya** if you prefer a relatively compact, neutral structure without a separate narrative persona.
- **Choose Eveline** if you prefer a layered structure with a distinct backstage narrative identity and more explicit guidance for continuity, world agency, scene texture, and adult intimacy.
- Back up your current Tavo preset before importing.
- Download the published version from the [GitHub Releases page](https://github.com/AozoraCynthiAStudio/Aozora-Tavo-Novel-Presets/releases), then import the JSON file into Tavo and check prompt slots, enabled states, and ordering.
- For source inspection or customization, browse [Iveya's JSON](presets/Iveya-Zhiyu-1.0.2.json) or [Eveline's JSON](presets/Eveline-Zhijing-1.0.2.json).

## Compatibility, feedback, and license

Results vary with the model, API provider, character cards, lore, history length, and generation settings. Neither preset guarantees a fixed response length, first-person narration, or identical behavior across models. Eveline's more layered structure may be followed differently by different models; additional rules do not guarantee better writing.

Feedback and reproducible issue reports are welcome and will inform future iterations, though not every suggestion will necessarily be adopted. This is an independent community project, not an official Tavo project or an endorsement by Tavo or any model provider.

Current preset version: **1.0.2**. Licensed under the **MIT License**; see [LICENSE](LICENSE).

<div align="center">

Made for more vivid, continuous interactive storytelling.

</div>