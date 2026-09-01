# WCJ-floorplan-style-render

WorkBuddy skill: 户型图风格渲染提示词生成器 —— 输入一张 2D 户型线稿图，输出专供 Nano Banana 的英文生图提示词（含逐段中文对照）。

## 安装

把整个目录放进 WorkBuddy 的 skills 目录即可：

- Windows: `C:\Users\<用户名>\.workbuddy\skills\`

安装后目录名保持 `WCJ-floorplan-style-render`。

## 目录结构

| 文件 | 说明 |
|---|---|
| `SKILL.md` | 技能主文件：分阶段流程 + 全部铁律 |
| `_user_meta.json` | 技能元数据 |
| `assets/example-reference-style.jpg` | 默认参考风格图（暖调极简奢宅） |
| `references/material-palette.md` | 材质调色板 |
| `references/style-decoding-guide.md` | 风格解码指南 |

## 工作流

1. 阶段一：识别线稿中的全部空间，列出清单等用户确认
2. 阶段二：确认后生成整段英文提示词 + 逐段中文翻译，一次性输出

## 默认风格

暖调极简奢宅（warm minimalist luxury）：浅蜜色橡木人字拼地板、奶油哑光墙面、深青铜灰哑光烤漆柜体、象牙白亚光石材台面、原生奶油色亚麻布艺、棕褐色皮革、厚实胡桃木、深青铜拉丝五金、米白无缝背景、左上方柔和漫射光。
