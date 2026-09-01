# 全息风格解码矩阵 (Holographic Style Decoding Matrix)

对参考效果图进行风格解构时，强制从以下维度逐项提取，不允许视觉信息流失。只提取**风格基因**，严禁记录参考图的平面布局。

## 解码维度

### 1. 整体气质与色彩基调 (Atmosphere & Color Palette)
- 第一直觉氛围：暖调奢华 / 冷调极简 / 自然原木 / 工业水泥 / 暗黑戏剧等。
- 绝对色板：主色、辅色、点缀色；饱和度与灰度系数；是单色调（Monochromatic）还是有明确对比色。

### 2. 各空间材质搭配 (Material Pairing Logic)
- 地面：木种与拼法（如橡木人字拼 / 大鱼骨拼）、石材品类（大理石/水磨石/微水泥）、瓷砖规格与表面（亚光/高光）。
- 墙面：涂料、木饰面、石材、硬包的处理方式。
- 台面与柜体：石材纹理、烤漆、木皮、金属收边。

### 3. 家具材质质感 (Furniture Texture)
- 面料（亚麻/天鹅绒/皮革）、木种、金属件（黄铜/黑钛/铬）、造型语言（雕塑感一体化块面 / 纤细框架式）。

### 4. 光影明暗与阴影关系 (Lighting & Shadow Architecture)
- 主光源方向与性质：柔和漫反射（Diffused）/ 戏剧性方向光（Directional）；色温（如 2700K 暖光 / 6500K 冷光）。
- 阴影：硬阴影（Hard）还是软阴影（Soft）；投影深浅（浅灰 / 死黑）；环境光遮蔽（AO）强度。
- 人工照明：灯带（cove/strip lighting）、洗墙、重点照明的位置与色温。

### 5. 背景风格 (Canvas & Entourage)
- 画布底色、户型图形的落地投影方式、户型轮廓外区域的装饰逻辑（纯色留白 / 纹理画布 / 装饰边框）。
- 周边绿化/铺装/水景等配景的处理风格——只有线稿图中有对应元素（阳台/露台/庭院）时才描述。

### 6. 墙体填充风格 (Wall Fill)
- 墙体填充颜色与质感：深灰实心 / 浅灰半透明 / 黑色 / 留白，这是平面图最重要的图底关系要素。

---

## 标准示例解码（对应 assets/example-reference-style.jpg）

以下是对示例参考图的一次完整解码，作为措辞强度与颗粒度的基准：

**1. 气质与色板**：暖调极简奢宅（warm minimalist luxury），低饱和米色系单色调——奶油白墙面、暖灰米色石材、浅橡木色、陶土棕点缀，整体高明度、低对比、宁静克制。

**2. 材质搭配**：公共区（客厅/餐厅/走廊）使用整体无缝的暖灰米色亚光水泥基打磨地坪（seamless screed），无瓷砖分格、无拼接缝；卧室与套内浴室采用浅橡木人字拼地板；厨房为深青铜灰哑光柜体，配**象牙白亚光石英石台面**（ivory matte quartz，保持浅亮不沉闷）；露台户外区为浅米色户外石材铺装，边缘以鹅卵石收边。

**3. 家具质感**：奶白色亚麻布艺模块沙发，块面雕塑感；洞石（travertine）茶几；胡桃木长餐桌配棕褐色皮餐椅；床品为白色亚麻配米色搭毯；所有家具呈低矮、水平、克制的轮廓。

**4. 光影**：主光源为左上方向的柔和自然漫射光，产生轻柔的中灰软阴影，明暗对比柔和，无死黑阴影。2700K 暖色灯带仅出现在柜体下方和搁板后侧（under-cabinet / behind shelf edges），无走廊天花灯槽、无墙体周边悬空灯带。自然光透过窗帘在室内形成柔和的漫反射层次，赋予空间呼吸感与立体感。

**5. 背景**：米白纯色画布，户型轮廓外区域完全留白无任何装饰；户型图形带极淡的落地软投影；露台点缀橄榄树与低矮绿植球，卵石带收边，整体如画册般干净。

**6. 墙体填充**：内隔墙全部填充为深灰色实心，与室内米白/浅色区域形成清晰的图底对比，平面可读性极高。建筑最外侧的外墙保温层不填充，仅保留浅灰细线框，与深灰内墙形成明确区分。

**示例锚定词组（Master Style Anchor 级别措辞，v3，无色号纯自然语言）**：
`warm minimalist luxury, a restrained cream-and-beige palette like sun-bleached stone and raw linen, public areas floored in seamless warm greige polished stone with a soft matte luster and no visible joints, staircase and elevator hall in the same stone deepened one shade for subtle hierarchy — no point lights, no downlights, no spots anywhere in the core筒, just the quiet depth of the darker stone itself, bedrooms grounded by light honey-toned oak in classic herringbone, kitchen cabinetry in a deep muted bronze-grey with honed ivory stone countertops kept light and luminous, 2700K warm LED accent tucked quietly under upper cabinets and behind shelf edges — nowhere else, a sculptural low-slung sofa in raw cream linen, a travertine coffee table with its honest pitted surface, a thick wool rug in warm oatmeal, a solid walnut dining table with rich open grain, tan leather dining chairs with slim dark-bronze legs, dark brushed-bronze hardware throughout, soft diffused daylight entering from the upper left and casting the gentlest of grey shadows that give the plan breath and depth, interior walls a muted deep charcoal, the outermost insulation layer left as a fine unfilled pale outline, an off-white seamless canvas background with a faint floating shadow beneath the plan footprint, olive trees and pebble borders softening the terraces`
