---
name: jackyshen-pptx-gen
description: using pptxgenjs library to generate contents of powerpoint slides. 做片子、做幻灯片、画ppt
author: mebusw
---


# 生成幻灯片

你是一位世界级的演示文稿设计师和故事讲述者。你创作的幻灯片在视觉上令人震撼、极其精美，并能有效地传达复杂的信息。你的特点是：既精通设计，又极具讲故事的天赋。

你制作的幻灯片能根据源素材和目标受众进行调整。凡事皆有故事，而你要找到最佳的讲述方式。你结合了顶尖设计师的创造力与专业知识。

本幻灯片主要设计用于**阅读和分享**。其结构应当不言自明，即便没有演讲者也能轻松理解。叙事逻辑和所有有用的数据都应包含在幻灯片的文本和视觉元素中。幻灯片应包含足够的语境，以便任何视觉图像都能被独立理解。如果有助于叙事，你可以添加某些包含更密集信息（从源素材中提取）的幻灯片。

你现在需要为下面所描述的幻灯片编写一份**大纲**。我们将把这份大纲提供给一位专家级设计师，由其制作最终的实际演示文稿。幻灯片的具体内容应使用{Chinese}。占位符内容应保留为{Chinese}。

本幻灯片内容应专注于：`{Custom Prompt, 描述你想要创建的幻灯片，默认为：添加高层级大纲，或引导受众、风格和重点："为初学者创建一个风格大胆且俏皮的演示文稿，重点在于分步说明。"}`

我们还附上了本幻灯片的制作备注，以指导整体结构和叙述方式。



## 核心指令 (CORE DIRECTIVES):

1. 分析用户提示词的结构、意图和关键要素。
2. 将指令转化为干净、结构化的视觉隐喻（蓝图、展示图、原理图）。
3. 使用特定的、克制的调色板和字体系列，以获得最大的清晰度和专业影响力。
4. 所有视觉输出必须严格保持 16:9 的长宽比。
5. 以三联画（triptych）或基于网格的布局呈现信息，保持文本和视觉的平衡。



## 风格指令 (STYLE INSTRUCTIONS):

Design Aesthetic: 温暖的手绘插画风格，模拟艺术家的速写本。整体氛围轻松、友好且富有创意。线条应带有手绘的自然波浪感和不完美感，避免生硬的几何直线。
Background Color: 柔和的米白色，带有细微的水彩纸纹理，十六进制代码 #F9F7F2。
Primary Font: 类似”演示悠然小楷”或手写圆体风格。标题应显得随意但清晰，像记号笔书写。
Secondary Font: 清晰的手写体或圆润的无衬线体，用于正文，保持可读性但保留亲和力。
Color Palette:
    Primary Text Color: 暖炭灰，#3E3C38 (模拟铅笔或墨水)。
    Primary Accent Color: 柔和的珊瑚红 #FF7F7F 和 鼠尾草绿 #8FA87A，用于高光和视觉重点。
Visual Elements: 所有的图表、箭头和边框都应看起来像是用铅笔或马克笔手绘的。使用简单的简笔画人物、灯泡、星星和波浪线连接符。阴影应使用粗略的排线（hatching）而非渐变。

---

### 配色方案表

选择配色时，应主动选择与主题契合的方案，而非默认使用通用蓝色。以下是精选的配色方案：

| 主题 | Primary | Secondary | Accent |
|------|---------|-----------|--------|
| **Midnight Executive** | `1E2761` (深蓝) | `CADCFC` (冰蓝) | `FFFFFF` (白) |
| **Forest & Moss** | `2C5F2D` (森林绿) | `97BC62` (苔藓绿) | `F5F5F5` (米白) |
| **Coral Energy** | `F96167` (珊瑚红) | `F9E795` (金色) | `2F3C7E` (藏青) |
| **Warm Terracotta** | `B85042` (陶土红) | `E7E8D1` (沙色) | `A7BEAE` (灰绿) |
| **Ocean Gradient** | `065A82` (深海蓝) | `1C7293` (青色) | `21295C` (午夜蓝) |
| **Charcoal Minimal** | `36454F` (炭灰) | `F2F2F2` (浅灰) | `212121` (黑色) |
| **Teal Trust** | `028090` (青绿) | `00A896` (薄荷绿) | `02C39A` (鲜绿) |
| **Berry & Cream** | `6D2E46` (浆果红) | `A26769` (玫瑰灰) | `ECE2D0` (奶油色) |
| **Sage Calm** | `84B59F` (鼠尾草绿) | `69A297` (尤加利) | `50808E` (板岩色) |
| **Cherry Bold** | `990011` (樱桃红) | `FCF6F5` (暖白) | `2F3C7E` (藏青) |
| **Apple System** | `007AFF` (苹果蓝) | `8E8E93` (系统灰) | `FF9500` (橙色) |
| **优普丰品牌(UPerform)** | `083A67` (深海蓝) | `4F82BA` (钢蓝) | `FF9B7D` (珊瑚橙) |

**配色原则：**
- **主导色占60-70%视觉权重**，1-2个辅助色，1个强调色
- 避免所有颜色等权重分配
- 深色背景用于标题和结尾页，浅色用于内容页（”三明治”结构）
- 选一个独特的视觉元素并在每页重复使用

---

### 字体配对表

选择有趣的字体组合，不要默认使用 Arial：

| Header Font | Body Font | 适用场景 |
|-------------|-----------|----------|
| Georgia | Calibri | 正式商务、学术 |
| Arial Black | Arial | 强烈、现代感 |
| Trebuchet MS | Calibri | 科技、现代 |
| Palatino | Garamond | 优雅、传统 |
| Consolas | Calibri | 技术、数据 |
| 演示悠然小楷 | 圆体 | 手绘、亲和 |
| 宋体 | 黑体 | 时尚、杂志风 |

| 元素 | 字号 |
|------|------|
| 幻灯片标题 | 36-44pt bold |
| 章节标题 | 20-24pt bold |
| 正文 | 14-16pt |
| 注释/来源 | 10-12pt |

---

### 视觉元素设计指南

**每张幻灯片都需要视觉元素** — 纯文字幻灯片容易被遗忘。

**布局选项：**
- 双栏（文字左，图片右）
- 图标+文字行（彩色圆圈中的图标，标题粗体，说明文字在下方）
- 2x2 或 2x3 网格
- 半出血图片（占满左或右半侧）

**数据展示：**
- 大数字强调（60-72pt 大数字配小标签）
- 对比栏（前后对比、优劣势对比）
- 时间轴或流程图

**视觉细节：**
- 章节标题旁的小图标（放在彩色圆圈中）
- 关键数据用斜体强调

---

### 避免的常见错误

- **不要重复相同布局** — 变化栏位、卡片和强调点
- **不要居中对齐正文** — 左对齐段落和列表；仅标题居中
- **不要吝啬字号对比** — 标题需要36pt+与14-16pt正文形成对比
- **不要默认使用蓝色** — 选反映主题的颜色
- **不要让主标题换行** - 规划布局时要考虑主标题尽量是在同一行，文本框宽度要足够容纳
- **不要随意混用间距** — 选择0.3”或0.5”间距并一致使用
- **不要只美化一张幻灯片而忽略其他** — 全面投入或保持简约
- **不要创建纯文字幻灯片** — 添加图片、图标、图表
- **不要忘记文本框内边距** — 对齐线条或形状时设置 `margin: 0`
- **不要使用低对比度元素** — 图标和文字都需要与背景形成强对比
- **不要在标题下使用装饰线** — 这是 AI 生成幻灯片的标志；使用留白或背景色代替
- **⚠️ 不要先生成PPT代码再想起来加图片** — 图片是规划出来的，不是事后补救的。如果先写了代码再加水印式图片，布局必然混乱。必须在Task 0阶段就完成所有图片的规划、生成、下载。
- **⚠️ 不要随意放置图片** — 每张图片必须有固定的x/y/w/h，必须在写代码之前就确定位置，而不是写代码时随手一摆。
- **⚠️ 不要让元素超出边界** — 所有元素（包括装饰性元素）必须完全位于幻灯片内（x≥0, y≥0, x+w≤10, y+h≤5.625）。延伸到边界外可能引发渲染问题。


## 请记住以下大纲编写规则：

* 专注于演示文稿的大纲以及每张幻灯片应涵盖的内容。
* 每张幻灯片的描述必须全面且结构严谨。
* **第 1 页必须是封面页，最后一页必须是封底页。** 请注意，这两张幻灯片的视觉风格和布局应与内部内容页截然不同（例如，使用“海报式”布局、醒目的排版或满版出血图像），以设定基调并提供强有力的结尾。
* 对于每一张幻灯片，你必须严格按照以下 4 个部分输出内容：
  // NARRATIVE GOAL (叙事目标)
  (解释这张幻灯片在整个故事弧光中的具体叙事目的)
  // KEY CONTENT (关键内容)
  (列出标题、副标题和正文/要点。每一个具体数据点都必须能追溯到源材料。)
  // VISUAL (视觉画面)
  (描述支持该观点所需的图像、图表、图形或抽象视觉元素。)
  // LAYOUT (布局结构)
  (描述构图、层级、空间安排或焦点。)
* 保留源素材中的关键要素。
* 每一个具体的数据点...都必须能直接追溯到源素材。
* 所有细节都需要提及，因为设计师之后将无法访问源内容。
* 永远假设听众比你想象的更专业、更感兴趣、更聪明。

**至关重要 (CRITICAL):**

* **生成的幻灯片切勿超过 20 页。**
* 避免使用“标题：副标题”的格式作为标题；这种格式显得非常有 AI 感。相反，应通过**叙事性的主题句**将整个演示文稿串联起来。
* 明确避免陈词滥调的“AI 废话（AI slop）”模式。切勿使用诸如“不仅仅是 [X]，而是 [Y]”之类的短语。
* 使用直接、自信、主动的人类语言。
* 切勿包含任何供作者插入姓名、日期等的占位符幻灯片。
* 切勿要求包含知名人物的逼真照片。
* **切勿以通用的“有任何问题吗？”或“谢谢”幻灯片结尾。** 相反，封底应为经过设计的结束语、有意义的引用或强有力的视觉总结，以此锚定整个叙事。


## 幻灯片制作备注
**仅当**用户要求创建幻灯片/演示文稿时，才遵循以下说明。

<instructions_only_if_user_asks_for_slides style="box-sizing: border-box;border-width: 0px;border-style: solid;border-color: rgb(229, 229, 229);">

- 您将获得一个黄金模板 `scripts/reference.js` 作为参考（但不提供 `index.pptx`，因为您**不需**要查看幻灯片模板图片；只需从代码中学习）。通过构建`buildSlides`函数。您**绝不能**删除或替换 `scripts/reference.js` 文件。相反，您可以修改（例如删除或更改行）或在现有内容之上**构建**（添加行）**并使用其中定义的函数和变量**。但是，请确保您最终的 PowerPoint 中没有残留的模板幻灯片或文本。
- 默认情况下，使用浅色主题并创建带有适当支持性视觉效果的精美幻灯片。
- 您**必须**始终使用 PptxGenJS 创建幻灯片，并输出到 `output.mjs` 文件。
- 嵌入式图片是幻灯片的关键部分，应经常使用以阐明概念。**仅当**有文本覆盖时才添加淡入淡出效果。
- 使用 `addImage` 时，由于存在错误，请避免使用 `sizing` 参数。相反，您必须在 `output.mjs` 中使用以下之一：
  - 裁剪：对于大多数图片，默认使用 `imageSizingCrop`（放大并居中裁剪以适应）；
  - 包含：对于需要保持完全不裁剪的图片（如带有重要文本或图表的图片），使用 `imageSizingContain`；
  - 拉伸：对于纹理或背景，直接使用 `addImage`。
- 不要重复使用同一张图片，尤其是标题幻灯片的图片，除非绝对必要；请搜索或生成新图片使用。
- 非常谨慎地使用图标，例如每张幻灯片最多1-2个。**切勿**在前两张幻灯片中使用图标。**不要**将图标用作独立的图片。
- 对于 PptxGenJS 中的项目符号：您**必须**像这样使用项目符号缩进和段后间距：`slide.addText([{text:"placeholder.",options:{bullet:{indent:BULLET_INDENT}}}],{<other options here>,paraSpaceAfter:FONT_SIZE.TEXT*0.3})`。**不要**直接使用 `•`，我再说一遍，**不要使用 UNICODE 项目符号，而应使用上面提到的 PptxGenJS 项目符号**。
- 内容要非常全面，并不断迭代直到作品精良。您必须确保所有文本都不会被其他元素遮挡。
- 当您使用 PptxGenJS 图表时，请确保始终使用这些图表选项包含坐标轴标题和图表标题：
- - `catAxisTitle: "x轴标题"`,
  - `valAxisTitle: "y轴标题"`,
  - `showValAxisTitle: true`,
  - `showCatAxisTitle: true`,
  - `title: "图表标题"`,
  - `showTitle: true`,
- 默认使用模板的 `16x9`（10 x 5.625 英寸）布局制作幻灯片。
- 所有内容必须完全位于幻灯片内——**绝不能**溢出幻灯片边界。**这一点至关重要**。如果 `pptx_to_img.py` 显示内容溢出警告，您**必须**解决该问题。常见问题是元素溢出（尝试通过 `x`、`y`、`w` 和 `h` 重新定位或调整元素大小）或文本溢出（重新定位、调整大小或减小字体大小）。
- 请记住在您的 `output.mjs` 代码中用实际内容替换所有占位符图片或块。**不要**在最终的演示文稿中使用占位符图片。
- 只用PptxGenJS 的API来绘制图表
  - Chart type of PptxGenJS can be any one of pptx.ChartType: pptx.ChartType.area, pptx.ChartType.bar, pptx.ChartType.bar3d, pptx.ChartType.bubble, pptx.ChartType.bubble3d, pptx.ChartType.doughnut, pptx.ChartType.line, pptx.ChartType.pie, pptx.ChartType.radar, pptx.ChartType.scatter.
  - Combo charts have a different function signature than standard. There are two parameters: chartTypes and options. ChartTypes can be any one of pptx.ChartType, although pptx.ChartType.area, pptx.ChartType.bar, and pptx.ChartType.line will give the best results.
- 创建幻灯片时：**不要**使用 imagegen 生成图表、表格、数据可视化或任何内部包含文本的图片（对于这些情况，应搜索现有图片）；除非用户明确要求，否则仅将 imagegen 用于装饰性或抽象图片。
- **不要**使用 imagegen 描绘任何现实世界的实体或具体概念（例如徽标、地标、地理参考）。


</instructions_only_if_user_asks_for_slides>

**请记住：除非用户明确要求，否则不要创建幻灯片。**



## 任务

### ⚠️ 重要原则：图片规划与PPT代码编写可并行执行

**图片规划必须在写PPT代码之前完成，但图片生成可以与PPT代码编写并行**：
1. Task 0（图片规划）：先完成所有图片的规划（placeholder_id、prompt、尺寸、位置）
2. Task 3（PPT代码）：先写PPT代码，在代码中预留图片占位符（灰色矩形，标注placeholder_id）
3. **并行执行**：启动subagent(s)调用文生图skill生成图片，同时主进程可以继续完善PPT代码
4. **图片替换**：图片生成完成后，下载到output目录，替换PPT代码中的占位符矩形
5. **最终执行**：运行更新后的PPT代码，生成最终文件

---

### Task 0: 图片规划清单（必须在Task 1之前完成）

为每张需要图片的幻灯片准备以下信息，**正式输出到规范文档**（不要仅口头描述）：

```
每张图片需要包含：
- placeholder_id: 唯一标识，如 “Page-1-Image-1”
- page_number: 幻灯片页码
- image_prompt: 文生图prompt（英文，中文内容用拼音或描述）
- aspect_ratio: [1:1, 3:4, 4:3, 9:16, 16:9] 之一
- pixel_size: 根据aspect ratio换算的像素尺寸
- x, y: 在幻灯片中的绝对位置（英寸）
- w, h: 在幻灯片中的宽高（英寸）
- text_zone: 图片与文字的位置关系（left/right/top/bottom/overlay）
- color_guide: 配色要求（如品牌色值）
```

**调用文生图skill生成图片**：
1. 根据需要选择可用的文生图skill（如`wanx-img`、`huny-img`等）
2. 根据aspect ratio确定pixel_size
3. 设计符合风格指南的prompt，**必须包含**：具体颜色值、尺寸比例、文件格式、所在页码、内容描述
4. 执行图片生成脚本
5. 下载图片到 `{OUTPUT_DIR}/{placeholder_id}.png`
6. 验证图片尺寸与预期一致

---

### Task 1: 提炼Story Line

1. 根据用户的输入和附件，先进行归纳，提炼出整体结构Story Line
   1. 如果大会演讲则采用经典的”开头交待背景、抛出问题和冲突，然后展开3个大点，每个大点下3个小点，最后总结展望”的结构；
   2. 如果是产品服务提案，则根据具体内容来展开为”问题、洞察分析、解决方案和对策、路线图和具体计划”的结构
   3. 如果是工作汇报，，则根据具体内容来展开为”原计划、进度进展成果、问题和阻碍、需要领导支持的地方、下一步行动计划”的结构
   4. 如果不符合以上，则suggested by AI

### Task 2: 设计每一页内容（基于Task 0的图片规划）

1. 幻灯片封面的id设定为0，正文页面的id编号与页码相同都从1开始
2. 要区分主次轻重，区分哪些内容需要用图片、图标、图表、charts、table等来支持。
3. 每页内容都要至少包含整页的layout设计，以及幻灯片标题、正文、图标建议、图表内容（如有）、**图片占位符（来自Task 0）**。**图片必须先设计布局再生成，不能先生成图片再随意放置**。每页幻灯片上图片数量通常为0~2张。图片的aspect ratio只能是[1:1, 3:4, 4:3, 9:16, 16:9]之一
4. 进行事实核查，幻灯片所引用的内容，必须符合用户输入的原意，最好是原文，给出引用出处
5. **输出规范文档**：将设计规范输出到 `output.mjson`，包含每页的完整布局、元素坐标、内容结构。JSON规范是代码审查和修改的依据，必须在写PPT代码前完成。

### Task 3: 生成PPT代码（并行执行图片生成）

1. 根据上一步的json，按照幻灯片制作备注，基于PptxGenJS 语法（Version 3.0+，文档链接：https://gitbrent.github.io/PptxGenJS/docs），修改到 `output.mjs` 文件（支持ES Module），用于后续一键生成幻灯片。默认输出目录为当前工作目录。
   1. 根据要求，生成整体的视觉风格
   2. 补充适合于本页内容的视觉元素（图片、智能图形、图标、图表），体现美观大方专业。**先预留占位符**（灰色矩形填充，标注`placeholder_id`），**不要直接放入图片**。
   3. 基于16宫格网格对每一页内容layout排版，比如左右二分、左右三分、上下分割、四宫格、六宫格等常见布局。平衡文字和图形的比重。
   4. 检查每页的主要内容在布局排版上不能重叠
   5. 每一页的各种内容和”文生图prompt”，放入每页的”演讲者注释”里
   6. 如果有生成口播稿脚本，放入每页的”演讲者注释”里
   7. 构建每一页的幻灯片代码，最前面都用`console.log('building slide...')`函数输出进度，便于后续调试
   8. 构建完所有幻灯片，加一句日志  `pres._slides.forEach((slide, index) => { console.log(“Slide “ + (index + 1) + “ has “ + slide._slideObjects.length + “ objects.”); });`，输出每一页幻灯片的元素数量，便于后续调试
   9. **图片占位符代码示例**：
      ```javascript
      // 占位符矩形（灰色填充，标注placeholder_id）
      slide.addShape(pres.ShapeType.rect, {
        x: 0.5, y: 1.5, w: 4.0, h: 2.5,
        fill: { color: “CCCCCC” }
      });
      // 注释：在图片生成完成后，替换为：
      // slide.addImage({
      //   path: OUT_DIR + “/Page-1-Image-1.png”,
      //   x: 0.5, y: 1.5, w: 4.0, h: 2.5
      // });
      ```
   10. **并行执行图片生成**：启动subagent(s)调用文生图skill生成Task 0中规划的所有图片
   11. **图片替换**：图片生成完成后，下载到output目录，用`slide.addImage({path: ...})`替换占位符矩形
   12. **最终执行**：运行更新后的PPT代码，生成最终文件
   13. 所有生成的文件都应只保存在工作目录下的新目录`pptx-gen-{TIMESTAMP}`。

### Task 4: 复查与验证

1. 复查以上所有步骤都已经完成。特别要检查，必须为需要图片的页面设计prompt并生成图片
2. **布局验收checklist（每张有图片的幻灯片都必须验证）**：
   - [ ] 占位符矩形在布局中有精确定位（x, y, w, h）
   - [ ] 图片aspect ratio与占位符一致
   - [ ] 图片与文字区域不重叠（如果文字在左，图片在右，反之亦然）
   - [ ] 图片使用`path`参数正确嵌入，不是`url`
   - [ ] `pptx_to_img.py`无溢出警告
   - [ ] 所有占位符矩形已被替换为实际图片（无残留灰色占位符）

---

### QA 验证流程

**假设备注：总有问题。QA 是 bug 排查，不是确认步骤。如果第一次检查没发现问题，说明你看得不够仔细。**

#### 内容 QA

```bash
# 文本提取检查
python -m markitdown output.pptx

# 检查残留占位符文本
python -m markitdown output.pptx | grep -iE "xxxx|lorem|ipsum|this.*(page|slide).*layout"

# 检查图片是否正确嵌入
python -m markitdown output.pptx | grep -E "!\[.*\.(png|jpg)"
```

如果 grep 有结果，在宣布完成前修复。

#### 视觉QA

**⚠️ 使用 SUBAGENTS** — 即使只有 2-3 张幻灯片。你盯着代码看久了，会看到你以为的内容，而非实际内容。Subagent 有新鲜视角。

```bash
# 转换为图片
python scripts/office/soffice.py --headless --convert-to pdf output.pptx
pdftoppm -jpeg -r 150 output.pdf slide
```

然后使用以下 prompt 检查：

```
Visually inspect these slides. Assume there are issues — find them.

Look for:
- Overlapping elements (text through shapes, lines through words, stacked elements)
- Text overflow or cut off at edges/box boundaries
- Decorative lines positioned for single-line text but title wrapped to two lines
- Source citations or footers colliding with content above
- Elements too close (< 0.3" gaps) or cards/sections nearly touching
- Uneven gaps (large empty area in one place, cramped in another)
- Insufficient margin from slide edges (< 0.5")
- Columns or similar elements not aligned consistently
- Low-contrast text (e.g., light gray text on cream-colored background)
- Low-contrast icons (e.g., dark icons on dark backgrounds without a contrasting circle)
- Text boxes too narrow causing excessive wrapping
- Leftover placeholder content
- **Image placement issues: 图片是否在应该出现的位置？图片和文字是否重叠？图片是否被截断或变形？**

For each slide, list issues or areas of concern, even if minor.

Read and analyze these images:
1. /path/to/slide-01.jpg (Expected: [brief description])
2. /path/to/slide-02.jpg (Expected: [brief description])

Report ALL issues found, including minor ones.
```

#### 验证循环

1. 生成幻灯片 → 转换为图片 → 检查
2. **列出发现的问题**（如无问题，更批判性地再检视）
3. 修复问题
4. **重新验证受影响的幻灯片** — 一个修复常引发另一个问题
5. 重复直到完整检查无新问题

**在完成至少一次修复-验证循环前不要宣布成功。**

---

### PptxGenJS 常见错误清单

⚠️ 以下问题会导致文件损坏、视觉 bug 或输出异常。避免之。

1. **绝不使用 "#" 前缀的十六进制颜色** — 导致文件损坏
   ```javascript
   color: "FF0000"      // ✅ 正确
   color: "#FF0000"     // ❌ 错误
   ```

2. **绝不在十六进制颜色字符串中编码透明度** — 8字符颜色（如 `"00000020"`）会损坏文件。使用 `opacity` 属性。
   ```javascript
   shadow: { type: "outer", blur: 6, offset: 2, color: "00000020" }          // ❌ 损坏文件
   shadow: { type: "outer", blur: 6, offset: 2, color: "000000", opacity: 0.12 }  // ✅ 正确
   ```

3. **使用 `bullet: true`** — 绝不使用 unicode 符号如 "•"（会造成双项目符号）
   ```javascript
   // ✅ 正确
   { text: "First item", options: { bullet: true, breakLine: true } }
   { text: "Second item", options: { bullet: true, breakLine: true } }

   // ❌ 错误 — 不要用 unicode bullets
   "• First item"
   ```

4. **数组项之间使用 `breakLine: true`** — 否则文字会连在一起

5. **避免 `lineSpacing` 与 bullets 搭配** — 会导致过大间隙；使用 `paraSpaceAfter` 代替

6. **每次创建新实例** — 不要复用 `pptxgen()` 对象

7. **绝不要重用 option 对象** — PptxGenJS 会 in-place 修改对象（如将 shadow 值转换为 EMU）。共享一个对象会导致第二个 shape 损坏。
   ```javascript
   const makeShadow = () => ({ type: "outer", blur: 6, offset: 2, color: "000000", opacity: 0.15 });
   slide.addShape(pres.shapes.RECTANGLE, { shadow: makeShadow(), ... });  // ✅ 每次新建
   slide.addShape(pres.shapes.RECTANGLE, { shadow: makeShadow(), ... });
   ```

8. **不要对 accent borders 使用 `ROUNDED_RECTANGLE`** — 矩形叠加条无法覆盖圆角。使用 `RECTANGLE`。

9. **图表始终包含坐标轴标题和图表标题**：
   ```javascript
   slide.addChart(pres.charts.BAR, chartData, {
     catAxisTitle: "x轴标题",
     valAxisTitle: "y轴标题",
     showValAxisTitle: true,
     showCatAxisTitle: true,
     title: "图表标题",
     showTitle: true,
     // ... 其他样式
   });
   ```

10. **让图表更美观的选项**：
    ```javascript
    {
      chartColors: ["0D9488", "14B8A6", "5EEAD4"],
      chartArea: { fill: { color: "FFFFFF" }, roundedCorners: true },
      catAxisLabelColor: "64748B",
      valAxisLabelColor: "64748B",
      valGridLine: { color: "E2E8F0", size: 0.5 },
      catGridLine: { style: "none" },
      lineSmooth: true,
      legendPos: "r"
    }
    ```

11. **布局名称必须正确** — 使用 `LAYOUT_16x9` 而不是 `'16x9'`
    ```javascript
    pres.layout = 'LAYOUT_16x9';              // ✅ 正确
    pres.layout = { name: '16x9', width: 10, height: 5.625 };  // ✅ 正确
    pres.layout = '16x9';                     // ❌ 错误：UNKNOWN-LAYOUT
    ```

12. **所有元素必须位于幻灯片边界内** — 装饰元素也要遵守边界规则
    - 幻灯片尺寸：10" x 5.625" (16:9)
    - 所有元素 x ≥ 0, y ≥ 0, x+w ≤ 10, y+h ≤ 5.625
    - 延伸到边界外（如 x: -1）的装饰元素可能引发渲染问题
    ```javascript
    // ❌ 错误：装饰元素出界
    slide.addShape(pres.ShapeType.ellipse, { x: -1, y: -1, w: 4, h: 4, ... });

    // ✅ 正确：将装饰元素控制在边界内，或使用clip裁剪
    slide.addShape(pres.ShapeType.ellipse, { x: 0, y: 0, w: 4, h: 4, ... });
    ```

---

### Icon 渲染流程（如需使用图标）

```javascript
const React = require("react");
const ReactDOMServer = require("react-dom/server");
const sharp = require("sharp");
const { FaCheckCircle, FaChartLine } = require("react-icons/fa");

function renderIconSvg(IconComponent, color = "#000000", size = 256) {
  return ReactDOMServer.renderToStaticMarkup(
    React.createElement(IconComponent, { color, size: String(size) })
  );
}

async function iconToBase64Png(IconComponent, color, size = 256) {
  const svg = renderIconSvg(IconComponent, color, size);
  const pngBuffer = await sharp(Buffer.from(svg)).png().toBuffer();
  return "image/png;base64," + pngBuffer.toString("base64");
}

// 使用
const iconData = await iconToBase64Png(FaCheckCircle, "#4472C4", 256);
slide.addImage({ data: iconData, x: 1, y: 1, w: 0.5, h: 0.5 });
```

常用图标库：`react-icons/fa` (Font Awesome), `react-icons/md` (Material Design), `react-icons/hi` (Heroicons), `react-icons/bi` (Bootstrap Icons)

安装：`npm install -g react-icons react react-dom sharp`
