---
name: xxd-shop-010
description: "Create XXD Shop 010 white-background pop-out product label cards (电商白底跃出标签图) as finished PNGs from a product photo, product directory or product information, treating the bundled original brief as the sole aesthetic authority: one complete, tidy label card on pure white, the product set inside it with its most appealing part breaking naturally past the edge, and a scannable three-tier copy stack — lead-in line, product or flavour title, supporting English or benefit — plus at most a restrained badge. Copy the user supplies is treated as a plan the model may compress and re-tier without changing meaning, unless the user asks for it verbatim. Without user copy, it first drafts a sourced three-tier copy plan for the user to confirm before generating. Supports multiple ratios or exact sizes and several compositions per size. Use when the user invokes xxd-shop-010 or asks for 白底标签图、跃出标签、口味标签、卖点标签卡、详情页信息模块."
---

# XXD Shop 010｜白底跃出标签

用本次的商品图或商品信息，生成一张白底上的独立标签卡：商品嵌在标签里，最诱人的部分跃出标签边缘，交付 PNG。

每次生成前，完整读取 `references/original-prompt/zh-CN.md`。这份中文原始提示词是唯一的创作与审美权威；不总结、不翻译、不混用，也不用本文件、README、样张或其他编号替代它。

每次构建生图请求前，完整读取 `references/shop-runtime.md`，它是唯一的家族运行合同。本 Skill 不另写第二套美术指导或运行规则。

所有成品直接写进 `~/Desktop/xxd/xxd-shop-010/` 下新建的一个任务目录（或 `--out` 指定的根目录），不建子目录，不自动拼总览。

## 本编号覆盖条款

**原稿中的平台指令与样例主题已移除。** 原始文件首行的 `@创建图像`（另一平台的调用指令）和末尾的“本次主题：麒麟西瓜”（当时的样例商品）都已从归档原稿删去，见 `references/original-prompt/README.md`。商品永远由本次输入决定。

**文字默认按“文案方案”处理。** 原稿明确写了两条分支，本编号对家族默认改了两处：

- 用户没给文案：本编号启用家族的“起草文案方案”。样张里模型自己写的食品饮品文案反复出现“0 添加”“低酸”“天然纯净”这类没有出处的说法，所以 Agent 先按原稿的三层起草：顶部短引导语或口味印象词，中部商品名或口味名，下部辅助英文或一两条小卖点；内容按原稿的“这是什么、有什么特点、为什么值得选”，只写口味、口感、品类常识和用户给的信息。用户确认后按 `--text plan` 出图。用户明确要模型自己写（`--text prompt`）时，才按原稿让模型生成短文案。
- 用户给了文案：原稿要求“先分析文案结构与主次关系……允许在不改变核心意思的前提下压缩、整理、强化层级”。所以只写了 `--copy` 时，本编号按 `--text plan` 处理。
- 用户说“一字不改”“逐字使用”或写了 `--text exact` 时，才按准确文案逐字使用。

开始生成前用一句话说明本次采用的是哪一种，避免用户以为文案会被逐字照搬。

**白底就是白底。** 背景纯白或接近纯白，不加场景、桌面、渐变色块或投影地面；标签卡本身可以有轻微的立体感。交付的是可以直接嵌进详情页的独立信息模块，原稿明确排斥“像整张海报而不是标签卡”。

**跃出要真实。** 越出标签边缘的必须是商品本身最有吸引力的部分（剖面、果肉、泡沫、瓶口、主体一角），不是凭空添加的飞溅装饰。有商品图时，越界部分的形态与商品图一致。

**事实：** 文案方案里的事实照用；模型自己生成的文案只写口味、口感和品类常识，不写糖度、产地、等级、认证等数字或资质，除非 `--facts` 提供。

**追加验收：** 白底干净；标签轮廓完整清楚；商品确实越界，越界自然不生硬；视觉顺序是先商品、再主标题、再卖点；圆标或角标数量克制；文案没有冗长说明。

**写入提示词：** 以下句子原话放进交付块的“本编号约束”；其余覆盖条款由 Agent 执行与验收，不进入提示词。

- 背景纯白或接近纯白，不加场景、桌面、渐变色块或投影地面。
- 越出标签边缘的是商品本身最有吸引力的部分，不是凭空添加的飞溅装饰。

## 参考文件

- `references/shop-runtime.md`：家族运行合同（含文案方案模式）
- `references/original-prompt/zh-CN.md`：运行时使用的原始提示词
- `references/original-prompt/README.md`：译文索引、权威说明与删除记录
- `references/runtime-preferences.md`：交付偏好沿用
- `references/sample-workflow.md`：仅用于维护样张
- `scripts/configured_imagegen.py`、`scripts/shop_preferences.py`
- `scripts/clean_marks.py`：验收时抹掉品牌名旁多出来的 ®、™
