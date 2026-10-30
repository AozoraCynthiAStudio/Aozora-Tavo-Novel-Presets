<div align="center">

# Aozora · Tavo Novel Presets

**双生小说式描写预设 · Two Novel-Style Writing Presets for Tavo**

面向 Tavo 互动小说与角色扮演的两种叙事预设。它们共享小说式描写、剧情连续性与场景表现的目标，但在提示词结构和叙事身份上采用不同路线。

Two narrative presets for interactive fiction and roleplay in Tavo. They share a novel-style writing foundation, with different approaches to prompt structure and narrative identity.

[![Version](https://img.shields.io/badge/version-1.0.4-5277C3?style=flat-square)](https://github.com/AozoraCynthiAStudio/Aozora-Tavo-Novel-Presets/releases/tag/v1.0.4)
[![License: MIT](https://img.shields.io/badge/License-MIT-2EA44F?style=flat-square)](LICENSE)

### 下载正式版 · Download

**[直接下载 1.0.4.zip（内含两份中文预设）](https://github.com/AozoraCynthiAStudio/Aozora-Tavo-Novel-Presets/releases/download/v1.0.4/1.0.4.zip)**

</div>

---

## 中文

## 项目定位与共同理念

Aozora · Tavo Novel Presets 是一组为 Tavo 互动小说体验设计的社区预设。我们关注的不只是“角色下一句说什么”，也包括玩家本轮提供的言行如何进入小说正文、人物如何通过动作与细节呈现，以及剧情如何在尊重玩家意图的前提下自然延续。

两份预设共享以下写作方向：

- **让玩家输入真正进入小说。** 将玩家本轮提供的戏内对白、动作和已确定的剧情事实自然写进正文开头，再接续其他角色的回应，而不是只让 NPC 听见或复述玩家的话。
- **把历史当作已经发生的故事。** 前文用于理解当前状态，不是每轮都要重写的素材。尽量避免无必要的剧情回顾、重复互动和已经发生过的情节重演。
- **让场景有层次和画面感。** 对话之外，适时描写人物位置、身体动作、眼神、表情、声音、停顿、空间关系与环境细节，让它们服务于人物和当下情境。
- **让人物与世界保持逻辑。** 角色依据自己的性格、经历和知情范围行动；世界可以自然运转，但不能为了显得主动就覆盖玩家已经确定的剧情方向。
- **让篇幅服从场景。** 重要互动可以充分展开，日常场景也可以轻松、安静或简短。不设固定最低字数，不为了显得文学化而灌水，也不要求每轮都发生重大变化。
- **保留玩家的创作空间。** 预设帮助故事更自然地写出来，但不应替玩家决定尚未给出的重大行动、感受或选择。

这些是写作风格与叙事组织方面的指导，不是模型升级、采样参数调整或 Tavo 引擎修改。实际表现会受到模型、API 服务、人物卡、世界书、上下文长度和生成设置影响。

## 两份预设的共同点与区别

| 对比项 | 伊薇娅·织语 | 伊芙琳·织境 |
|---|---|---|
| **共同目标** | 小说式接续、剧情连续性、人物细节与自然场景描写 | 小说式接续、剧情连续性、人物细节与自然场景描写 |
| **诞生顺序** | 后来整理出的适配版本 | 最初的自用原型 |
| **叙事身份** | 不额外设立独立叙事人格 | 有明确的高位叙事人格： “活着的编年者” |
| **提示词结构** | 相对简洁，接近 Tavo 常见的提示词槽位组织 | 规则分层更细，围绕既有模块体现叙事身份与职责 |
| **额外侧重点** | 以中性、通用的小说写作指导为主 | 在共同写作目标之外，包含面向明确成年虚构角色的亲密叙事指导 |
| **设计原因** | 为适应不接受额外人格或身份设定的中转站使用环境而整理 | 保留原本具有完整人格与叙事身份的设计 |
| **适合谁** | 希望使用中性结构、不希望预设带有独立叙事人格的玩家 | 希望保留伊芙琳的叙事人格、分层规则与亲密叙事指导的玩家 |

两份预设并不是基础版与高级版，也不保证某一份在所有模型上都更好。它们的实际输出可能非常接近，差异不一定每轮都明显。规则更多、人格更鲜明，并不意味着必然写得更好或更长。

**简单选择：** 如果你希望使用不带独立叙事人格、结构相对中性的版本，可以选伊薇娅；如果你希望保留我们最初设计的叙事人格与亲密叙事指导，可以选伊芙琳。

---

## 伊薇娅·织语

### 一句话定位

**不额外设立独立叙事人格，以相对简洁、中性的提示词结构，专注于小说正文、剧情连续性与场景表现。**

### 为什么会有伊薇娅？

最初我们先制作的是供自己使用的伊芙琳。后来，为了适应要求预设不带额外人格或身份设定的中转站，我们保留共同的小说式写作目标，整理出结构更中性的伊薇娅。

因此，伊薇娅不是因为写作能力较弱而产生的“低配版”，也不是把伊芙琳的所有规则机械删掉后得到的版本。她的定位是：不增加独立叙事人格，尽量用常规、简洁的提示词结构完成相同方向的写作指导。

### 它主要关注什么？

- 把玩家本轮的戏内对白和动作自然融入正文开头，允许润色表达，但不改变原本意图、顺序与结果。
- 让前文作为当前剧情的历史依据，减少重复叙述和无必要的回顾。
- 通过动作、眼神、表情、声音、停顿和环境细节丰富画面，而不是只依赖对白。
- 让人物关系与世界反馈基于已经发生的事情自然变化，不强迫每轮推进重大事件。
- 尊重玩家已经指定的剧情方向，不擅自替玩家决定行动或感受。

### 适用场景

- 希望聊天记录读起来更像连续的小说，而不是一问一答的对话。
- 希望改善动作、情绪和场景细节，但不想每轮都被强制扩写。
- 希望使用不带独立叙事人格、结构相对中性的预设。
- 使用环境对额外人格设定较敏感，希望尽量避免这类额外设定。

伊薇娅的目标是提高结构的通用性与中性程度，但这不构成对所有中转站或 API 服务的绝对兼容保证。具体要求仍应以服务商规则为准。

---

## 伊芙琳·织境

### 一句话定位

**拥有高位叙事身份的“活着的编年者”：她见证、记录、理解并展开故事，让人物、情绪与世界在既有事实的基础上继续流动。**

### 她是谁？

伊芙琳是我们最初为自己设计的版本。她不只是机械执行写作指令的后台工具，而是被赋予明确叙事身份的存在：站在故事整体的视角，理解人物经历、关系变化、未解决的事件和世界状态，再将这些信息组织成连贯的后续故事。

她的“高位”体现于理解、记录、组织和展开故事的叙事职责，并不意味着她可以随意覆盖玩家决定、改写人物卡与世界设定，或突破模型和服务平台的限制。

伊芙琳也不需要每轮向读者介绍自己。除非玩家明确选择与她本人互动，她默认在幕后工作，不闯入剧情、不抢走角色的位置，也不反复展示后台规则。她的身份应通过稳定的故事理解、准确的关系把握、合适的描写节奏和自然的世界反馈体现出来。

### 她的设计理念

伊芙琳的核心气质是成熟、温和、敏锐、有审美，也有自己的判断。

- **理性与情感并存。** 理性负责人物逻辑、世界规则与长线连续性；情感理解让关系、犹豫、亲近、失落与期待通过具体行为表现出来。
- **有判断力，但不夺取玩家的创作权。** 她可以连接剧情片段、选择值得展开的细节，让 NPC 在合理范围内主动回应；但不能替玩家决定未给出的重大行动。
- **让情绪落在具体场景里。** 通过动作、声音、停顿、视线、距离和互动反馈表现人物，而不是只给情绪贴标签。
- **懂得展开，也懂得留白。** 重要时刻可以写得细致，普通日常则可以平淡、幽默或简短，不强迫每轮发生重大心理变化。

简单来说：**理性负责不跑偏，情感负责让故事有温度。**

### 关于成年亲密叙事指导

伊芙琳还包含面向**明确成年人的虚构角色**的亲密叙事指导，重点是让关系与互动保持自然连续，而不是因进入亲密阶段就突然重置人物关系、切换成无关的说明口吻，或机械地重复同一种表达。

这些指导用于改善叙事方式，不是突破模型或 API 服务限制的技术模块，也不保证特定内容一定会被生成。模型和服务平台的规则仍然适用。

### 适用场景

- 希望使用具有明确叙事身份的版本，而不只是常规写作指令。
- 重视长线互动中人物经历、关系变化与事件后果的延续。
- 希望 NPC 和世界能在合理范围内主动回应，而不是每轮只给出一句回答。
- 希望场景细节、动作、情绪与人物关系形成更连贯的整体。
- 希望使用面向成年虚构角色的亲密叙事指导，并理解实际生成仍受模型和服务平台限制。

伊芙琳是我们的原始设计路线；伊薇娅则是为了适应不同使用环境而整理出的中性路线。两者的差异首先在叙事身份与结构选择，而不是谁一定能生成更好的文字。

---

## 下载、安装与修改

普通玩家请前往 [GitHub Releases](https://github.com/AozoraCynthiAStudio/Aozora-Tavo-Novel-Presets/releases)，下载正式附件 **1.0.4.zip**。解压后会看到两份中文预设：

- 伊薇娅·织语_1.0.4.json
- 伊芙琳·织境_1.0.4.json

建议先备份现有预设，再在 Tavo 中导入需要的 JSON，并用自己常用的模型、人物卡和世界书测试。仓库中的 JSON 文件也可供查看源码和自行修改。

## 兼容性与反馈

- 实际表现会受到模型、API 服务、人物卡、世界书、聊天历史长度和生成设置影响。
- 两份预设都不保证固定字数、第一人称叙述或跨模型完全一致的表现。
- 伊薇娅以中性和通用结构为设计目标，但不代表已经验证兼容所有中转站或 API。
- 伊芙琳包含更明确的叙事身份与分层规则，不代表它必然写得更好。
- 欢迎提交可复现的问题与使用反馈。社区反馈会作为后续迭代的参考，但不代表每项建议都会合并。

本项目为独立社区项目，不是 Tavo 或任何模型服务商的官方项目，也不代表其官方背书。

## 最新更新

**v1.0.3 · 2026-10-27**：尝试改善“今天、明天、后天”等相对时间表达在剧情推进中的连续性。该调整属于提示词层面的尝试，实际效果可能因模型与上下文而异。

## 版本与许可证

当前预设版本：**1.0.4**。

本项目使用 **MIT License**，详情见 [LICENSE](LICENSE)。你可以按许可证条款使用、修改和再发布；分享修改版时，请保留适用的版权和许可证声明。

---

## English

Aozora · Tavo Novel Presets offers two related presets for novel-style roleplay in Tavo. Both aim to integrate the player's latest in-story input into prose, maintain continuity, and build scenes through relevant actions, emotions, and environmental details.

| | Iveya Zhiyu | Eveline Zhijing |
|---|---|---|
| Origin | Created later for environments that prefer no additional persona identity | The original personal preset |
| Narrative identity | No separate narrative persona | Eveline, the “living chronicler,” with a distinct backstage narrative identity |
| Structure | More compact and neutral | More layered, with a clearer narrative identity |
| Additional focus | General novel-style writing guidance | Includes intimacy-writing guidance for clearly adult fictional characters |
| Best suited for | Users who prefer a neutral structure without an additional persona | Users who want the original narrative identity and additional intimacy guidance |

The presets share the same core writing goals and may produce very similar results. Neither is universally better, and neither guarantees compatibility with every model or provider.

Download **[1.0.4.zip](https://github.com/AozoraCynthiAStudio/Aozora-Tavo-Novel-Presets/releases/download/v1.0.3/1.0.3.zip)** from GitHub Releases. It contains both Chinese-named JSON presets. The project is MIT-licensed and community-maintained, not an official Tavo project.
