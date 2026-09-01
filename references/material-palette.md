# 材质色板（内部参考，不写入提示词） (Material Palette — Internal Reference)

此色板仅供内部对照材质匹配置信度，**色号绝不写入提示词**。提示词中一律使用自然语言质感描述。铁律逻辑（墙体填充、灯带绑定、核心筒加深、无缝地面、浅亮台面）始终强制，但同样以自然语言表达。

## 地面 (Floor)

| 编号 | 材质名称 | 色号 | 质感 | 典型写法 |
|------|----------|------|------|----------|
| F-01 | 暖灰米色微水泥 | #C4B7AC | warm greige polished micro-cement, seamless, no grout lines | `seamless warm greige polished micro-cement floor #C4B7AC` |
| F-02 | 浅橡木人字拼 | #C9A87C | light oak herringbone parquet, matte wood grain | `light oak herringbone parquet #C9A87C` |
| F-03 | 暖米色洞石 | #D2C5B3 | warm beige travertine, honed matte, subtle natural pitting | `warm beige travertine #D2C5B3` |
| F-04 | 深暖灰微水泥 | #A89E96 | darker warm taupe-grey micro-cement, seamless, one shade deeper than F-01 | `darker warm taupe-grey micro-cement floor #A89E96`（仅核心筒） |

## 墙体 (Wall / Fill)

| 编号 | 材质名称 | 色号 | 质感 | 典型写法 |
|------|----------|------|------|----------|
| W-01 | 深灰内墙填充 | #4A4A4A | dark grey solid fill, no texture, opaque | `dark grey solid fill #4A4A4A`（仅内隔墙） |
| W-02 | 外墙保温层 | N/A | thin pale grey unfilled outline only, no fill | `exterior insulation layer: thin pale-grey outline only, unfilled` |
| W-03 | 奶油白室内墙面 | #F5F0EA | cream-white matte paint, smooth | `cream-white matte wall #F5F0EA` |

## 柜体 / 台面 (Cabinetry & Countertop)

| 编号 | 材质名称 | 色号 | 质感 | 典型写法 |
|------|----------|------|------|----------|
| C-01 | 深青铜灰柜体 | #4A4845 | dark bronze-grey matte lacquer, concealed-grip hardware | `dark bronze-grey matte lacquer cabinetry #4A4845` |
| C-02 | 象牙白石英石台面 | #E8DFD5 | ivory matte quartz, subtle soft veining, light warm-beige tone | `ivory matte quartz countertop #E8DFD5`（必须用于所有厨房台面） |
| C-03 | 暖橡木木皮 | #C4A076 | warm oak veneer, matte wood grain | `warm oak veneer #C4A076` |

## 软装 / 家具 (Upholstery & Furniture)

| 编号 | 材质名称 | 色号 | 质感 | 典型写法 |
|------|----------|------|------|----------|
| U-01 | 奶油亚麻布艺 | #EBE3D8 | cream linen, coarse woven texture, sculptural low-slung | `cream linen sculptural sofa #EBE3D8` |
| U-02 | 棕褐色皮革 | #8B6E4E | tan leather, matte, fine grain | `tan leather dining chair #8B6E4E` |
| U-03 | 胡桃木实木 | #6B4F3A | solid walnut, matte, open-grain | `solid walnut dining table #6B4F3A` |
| U-04 | 深青铜金属件 | #5A5450 | dark-bronze metal, matte brushed finish | `dark-bronze matte brushed metal #5A5450` |
| U-05 | 燕麦色羊毛地毯 | #D6CFC4 | warm oatmeal thick-pile wool rug | `warm oatmeal wool rug #D6CFC4` |

## 背景 / 照明 (Canvas & Lighting)

| 编号 | 材质名称 | 色号 | 质感 | 典型写法 |
|------|----------|------|------|----------|
| B-01 | 米白画布背景 | #F4F4EF | off-white seamless canvas, pure solid color | `off-white seamless canvas background #F4F4EF` |
| L-01 | 2700K 暖光 | N/A | warm 2700K LED, soft point / linear glow | `2700K warm LED cove lighting`、`2700K warm wall sconce` |

## 用法

生成提示词时，每个空间内具体描述材质时必须带上色号，例如：

```
Living room: cream linen sculptural sofa #EBE3D8, travertine coffee table #D2C5B3,
warm oatmeal wool rug #D6CFC4, seamless greige micro-cement floor #C4B7AC.
```

这确保了不同户型、不同时间生图的材质色彩与质感完全一致。色板只覆盖风格提取最稳定的通用材料；如果参考图中出现色板未覆盖的材质（如特殊石材或金属饰面），按照色板的颗粒度新建一行补充，沿用至全提示词。

## 固定元素描述模板

### 灯带（仅用于柜体/台面绑定位置）
```
2700K warm LED strip under upper cabinets / behind shelf edges / under island counter.
严禁：ceiling perimeter, corridor cove, wall-top, 或任何无家具依附位置。
```

### 核心筒地面
```
Staircase and elevator hall: darker warm taupe-grey micro-cement floor #A89E96, one shade deeper than the interior public area floor #C4B7AC.
```
