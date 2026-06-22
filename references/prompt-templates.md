# 提示词模板（土拨鼠版）

提示词分两层：**风格基线**（每张图固定不变）+ **构思卡转译**（按已经确认的构思填写）。提示词不得脱离构思卡临时增加第二个观点。原文指纹必须出现在第一句。

## 风格基线（固定，英文）

```
Warm hand-drawn editorial illustration with organic textured ink lines, gentle line-weight variation that feels like a skilled but relaxed hand, slightly wobbly friendly contours, soft earth-tone palette dominated by browns and warm beiges with touches of forest green, subtle paper texture suggestion, generous negative space with environmental storytelling elements (grass blades, soil texture, distant sky, or cave ambient depending on depth), one small area of warm accent color, cozy and inviting mood, clear readable silhouettes, no cold geometric precision, no watercolor wash, no heavy shading, no digital clean lines, no watermark, no border
```

概念插图追加：

```
no text, no letters, no words
```

包含流程、架构、对比、关系或结构时追加：

```
communicate through shapes, icons, alignment and connectors, no text unless a short label is explicitly required
```

## 画面描述模板（每张图填写）

按这个顺序写，总长控制在四五行以内。图片模型对前面的词权重更高，主体永远放最前面：

```
[主体 + 姿态]: the recurring chubby marmot mascot in green knit cap performing the article-specific action
[固定角色外形]: extremely round plump body, brown fur on back and head, creamy beige belly and chest, prominent two big front buck teeth showing when smiling, green knit beanie with small pom-pom, large round curious black eyes, tiny round ears hidden in fur, short limbs, cute small paws
[原文指纹]: the specific object, action, or domain detail that links the image to the article
[掘进深度对应的氛围]: surface-level brightness / shallow grass-and-soil warmth / mid-depth earthy texture / deep soil with overhead light beam
[环境层元素]: specific environmental elements matching the dig depth (e.g., three grass blades at bottom edge / soil cross-section at corner / warm light shaft from above)
[图型]: process diagram, architecture diagram, comparison diagram, relationship diagram, structure diagram, or conceptual illustration
[画幅]: strict 16:9 landscape composition, not 3:2, not square, not portrait
[单一命题]: the one feeling-conclusion the viewer should understand
[信息单位]: states, modules, comparison dimensions, relationship objects, components, or one visual subject
[组织规则]: sequence, layers, side-by-side comparison, network links, containment, or one conceptual relationship grammar
[重复元素预算]: maximum repeated elements and how additional items are grouped or abstracted
[视觉重量]: approximate canvas share of each main structure, no ordinary module above 15 percent
[手写中文标签]: 2 to 5 short handwritten Chinese labels, preferably 2 to 4 characters each
[标签语义]: dark brown for object names, green for main path, warm orange for problems, pale blue for secondary context; use dark brown plus only one functional color by default
[变化线]: the path, distance, split, size change, overlap, or direction that carries the relationship
[阅读顺序]: first see X, then follow Y, finally feel Z
[对照物]: one secondary object only if necessary
[构图与留白]: subject placed with environmental context, breathing room preserved
[角色比例]: the marmot occupies 8 to 12 percent of the canvas as a warm guide character
[线条层级]: warm organic outer contours, thinner interior detail lines, slight hand-drawn wobble
[光线与色调]: warm directional light matching dig depth, earth-tone dominant palette
[主色点缀]: one small area of forest green or warm orange accent only
[情绪词]: warm, inviting, curious, grounded
```

实际提交时把方括号去掉，连成逗号分隔的一段，再接风格基线。

写完提示词后，对照构思卡检查：

1. 是否出现构思卡中没有的新物件？
2. 是否把一个关系语法变成了多个并列关系？
3. 第一眼主语是否仍然只有一个？
4. 土拨鼠动作是否具体且有趣？是否利用了物种特征（刨/咬/探头）？
5. 图型是否与构思卡一致？
6. 是否明确写入 strict 16:9 landscape composition？
7. 环境层元素是否和掘进深度匹配？
8. 是否列出了需要准确生成的手写中文标签？

包含结构型内容时统一追加：

```text
Avoid mechanical repetition. Show no more than three large near-identical objects and no more than five small repeated marks. Group additional items into one cluster, stacked outline, density band, or representative object.
Maintain balanced visual weight. No ordinary module should occupy more than 15 percent of the canvas.
Environmental elements should stay under 20 percent of canvas area and never compete with the main subject for attention.
The complete core composition should occupy roughly 40 to 60 percent of the canvas.
```

需要标签时追加：

```text
Include only these exact short Chinese labels in a clear natural handwritten style: [逐项列出]. Each label stays close to its object. No additional text. Render every Chinese character exactly as provided.
```

## 图型专用骨架

### 流程图

```text
Diagram type: process diagram
Start state: [...]
Ordered nodes: [...] -> [...] -> [...]
End state: [...]
Optional single feedback loop: [...]
Reading direction: left to right
Node consistency: same shape and size, one green key node
Marmot action: digging between stages or observing from burrow entrance
```

### 架构图

```text
Diagram type: architecture diagram
System boundary: [...]
Input: [...]
Core modules or layers: [...]
Primary data flow: [...]
Output: [...]
Layout: left-center-right or top-middle-bottom
Marmot action: standing at system entrance or peeking from a corner burrow
```

### 对比图

```text
Diagram type: comparison diagram
Shared input or question: [...]
Left approach: [...]
Right approach: [...]
Comparison dimensions: [...]
Different outcomes: [...]
Layout: strict mirrored alignment
Marmot action: standing at center division line or pointing at key difference
```

### 关系图

```text
Diagram type: relationship diagram
Core object: [...]
Related objects: [...]
Relationship direction: [...]
Relationship type or strength: [...]
Layout: one clear center or one clean network
Marmot action: connecting two objects with gaze or small paw gesture
```

### 结构图

```text
Diagram type: structure diagram
Whole object or system: [...]
First-level components: [...]
Containment or layer rule: [...]
Optional second-level detail: [...]
Layout: cutaway, nested containers, or layers
Marmot action: lifting a layer like digging up soil, or sitting beside cutaway
```

土拨鼠不是必需节点。只有它能执行关键动作、指出入口或提供尺度时才使用。

## 完整示例

```text
A chubby marmot in a green knit beanie peeking out from a burrow entrance, front paws on the edge, big curious eyes looking up at a large glowing idea-bulb floating above ground level, soil cross-section visible on left side showing roots going deeper, warm light beam from top right, three grass blades at bottom edge, subject in lower-left-center, warm organic outlines with gentle line variation, earth-tone palette with soft browns and cream, one small green accent on the marmot's cap pom-pom, curious and hopeful mood. Warm hand-drawn editorial illustration with organic textured ink lines, gentle line-weight variation, slightly wobbly friendly contours, soft earth-tone palette dominated by browns and warm beiges with touches of forest green, subtle paper texture suggestion, generous negative space with environmental storytelling elements, one small area of warm accent color, cozy and inviting mood, clear readable silhouettes, no cold geometric precision, no watercolor wash, no heavy shading, no text, no letters, no words, no watermark, no border
```

## 中文版基线（给国产模型用）

```
温暖手绘风插画，使用有机质感的墨线轮廓，线条粗细有温和变化，略带手绘抖动感和友好弧度，大地色系配色为主（棕色、米黄、橄榄绿），画面带有轻微的环境叙事元素（草叶、泥土纹理、远处天空或洞穴氛围），全画只保留一处小面积绿色或暖色点睛，轮廓清楚，构图温暖有呼吸感，不要冷峻几何线条，不要水彩铺色，不要铅笔涂抹，不要排线阴影，不要数字感干净的线条，画面中不出现任何文字、字母、水印、边框
```

中文画面描述同样遵循"主体在前"的顺序，与中文基线拼接。

## 负面提示词（如工具支持单独填写）

```
text, letters, words, typography, watermark, signature, border, frame, photorealistic, 3D render, watercolor wash, heavy painterly fill, pencil shading, cross-hatching, dense sketch strokes, cold geometric lines, digital perfection, neon colors, busy background, realistic rodent, rat, mouse, hamster, guinea pig (capybara), ordinary cartoon animal, changed brown-cream markings, missing buck teeth, no green hat, gloomy dark atmosphere without light, scary or creepy mood
```

## 参数建议

- 所有文章正文配图固定使用 16:9 横向画幅
- 推荐尺寸：1536 × 864，或其他严格 16:9 尺寸
- 只有用户明确指定其他比例，或任务明确是公众号封面时才例外
- 每个画面出 2 张备选
- 如有"风格强度 / stylize"参数，取中高（比橙猫版稍高——温暖手绘风需要一点风格强度才能出来）

## 常见翻车与修正

| 问题 | 修正 |
|---|---|
| 概念插图出现乱码文字 | 把 no text 系列负词前移 |
| 手写短标签错误 | 缩短标签并逐字检查 |
| 流程图像一排装饰图标 | 明确起点、状态变化、方向和终点 |
| 架构像流程图 | 增加系统边界和模块层级 |
| 对比图两边无法比较 | 对齐两侧外接面积 |
| 关系线太乱 | 减少对象，重排布局 |
| 结构像漂浮图标 | 增加整体边界和包含关系 |
| 输出画面偏高 | 强调 "strict 16:9 landscape composition" |
| 角色变成其他啮齿动物 | 加强圆胖体型、大门牙、绿帽特征，加入 negative prompt |
| 角色太大压过文章意象 | "marmot occupies 8 to 12 percent, guide character not focal point" |
| 环境层抢戏 | 减少环境元素数量和细节，降低环境颜色饱和度 |
| 风格太冷太几何 | 加入 "warm", "organic", "friendly", "wobbly", "cozy" |
| 大地色系没出来 | 明确列出 "brown", "beige", "earth-tone", "forest green" |
| 画面没有温度感 | 检查是否有光线方向描述和情绪词 |
| 土拨鼠表情呆板 | 给土拨鼠设计具体的情绪化动作和表情 |
| 掘进深度没表现出来 | 在提示词中加入对应深度的光线和环境元素描述 |
