# Pureza 素

### 这是干嘛用的？
Pureza 是一套用于生产纯色且简约风格的图像的提示词。

### 效果对比

| 原图 | 修改后 |
| :---: | :---: |
| <img src="assets/iris-original.webp" width="380"> | <img src="assets/iris-modified.webp" width="380"> |

（由 GPT Image 2.5 Sunburst - Low Quality Level 生成，该角色为原创角色“羽瞳”，采用 CC BY-NC-SA 4.0 协议发布）

| 原图 | 修改后 |
| :---: | :---: |
| <img src="assets/lumi-original.webp" width="380"> | <img src="assets/lumi-modified.webp" width="380"> |

（由 GPT Image 2.5 Sunburst - Low Quality Level 生成，该角色为原创角色“羽沁”，采用 CC BY-NC-SA 4.0 协议发布）

### 用在哪儿？

Pureza 适用于支持自然语言理解的 AI 图像生成模型。使用时，将其注入你的提示词便可。

若你的生图模型区分正向提示词和负向提示词，请关注即将更新的 “双向提示词（适用于 Stable Diffusion/NovelAI 等模型）”。

### 什么环境下使用它最合适？

笔者推荐在图像色彩偏向于颜色对立分明且附属颜色被并入主题颜色不会影响效果的情况下使用。

建议现版本不要在初次生成阶段就使用该提示词，如需生成阶段使用，后期将会发行适用于生成阶段版本的提示词。最推荐的使用方法应该是多次生成后在最后阶段使用或是有原图的情况下该提示词。

搭配该提示词的 AI 生图模型，笔者推荐使用 GPT Image 2、GPT Image 2.5 Flare 和 GPT Image 2.5 Sunburst。

目前不推荐使用 Nano Banana 系模型。经测试，该系列模型的两款主力模型（Nano Banana 2、Nano Banana 2 Lite）某些情况下（如使用中低质量生成）会导致严重的色彩偏移。高质量虽然色彩准确，但是效果不佳。

ByteDance Seedream 模型未经测试，目前尚不知晓。请谨慎使用。

### 关于图片生成模型的生成质量档位选择

对于 GPT Image 系列模型，生图质量档位提高并不会有太大收益。笔者的经验之谈，如果你用的是 API 接入而非 GPT 订阅，建议你为了成本选择 Low 档位。但是 Extra High 和 Max 档位会稍微改善质感。
对于 Nano Banana 系列模型，提高生图质量可以显著改善色彩采样导致的偏移问题。

### 关于中英文提示词差异

一般情况下，中英文提示词并无差异。某些极端情况下，建议使用中文提示词。中英文提示词因为翻译词汇的语义偏差问题，在某些细节上会有些差异。具体表现为中文提示词生成的图像风格会更干净利落并且出于不知名原因色彩采样会更准确。但是一般来说，中英文提示词两者之间并无差异。

### 提示词内容（中文，单图修改）

'''

请把这张图（图一）按照下文规则修改。
不要使用墨线，请直接使用色块！保持主体在全图中心的位置和纯色背景。强化“尽可能使用色块表达、化繁为简”的中心思想。将原图使用的颜色自行总结成最少两种最多10种（请尽量往3种、5种、8种的档位上靠），重绘使用的颜色只能用刚才总结的这几种，重绘使用的颜色出现得越少越好，色块整合得越统一越好。
画面完全由图形构成，没有文字、数字、字母、签名或水印；没有第二个人物；背景不出现渐变、场景或地平线；不画夸张的腮红与油亮高光；不性感化；整体干净、通透、飘逸。

'''

### 提示词内容（英文，单图修改）

'''

Please color and modify the main subject of this image (Image 1). Do not use ink outlines — use blocks of color directly. Keep the subject centered in the overall composition and keep a solid flat-color background. Reinforce the central principle: "express as much as possible through blocks of color; simplify the complex."
Summarize for yourself the colors used in the original image into no fewer than two and no more than ten (lean toward the tiers of 3, 5, or 8). The redraw may use only those summarized colors; the fewer times those colors appear, the better, and the more unified the merged color blocks, the better.
The image is composed entirely of shapes — no text, numbers, letters, signatures, or watermarks; no second figure; no gradients, scenery, or horizon line in the background; no exaggerated blush or glossy highlights; no sexualization; overall clean, luminous, and flowing.

'''

### 笔者的建议
建议不要在无原图版权的情况下使用该提示词进行对原图的二次修改！这条约束并没有强制力，但是只是笔者的一点建议。

### TODO 代办
- [ ] 普适性 Skill
- [ ] 生成阶段提示词
- [ ] 双向提示词
- [ ] Seedream 测试
---

本提示词基于 MIT 开源协议发布。

原始发布者：琦拉铃（Kirarin）
