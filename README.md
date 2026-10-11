# photo-skill

用于 AI image 模型的摄影师技能：将画面意图与参考图转成机位、构图、摆姿、用光、透视、景深和材质指令，支持生图、参考图编辑、系列图与提示词设计。

## 安装

将仓库文件放到 Codex 技能目录中的 `photo-skill` 文件夹，例如 `~/.codex/skills/photo-skill/`，确保其中直接包含 `SKILL.md`、`agents/` 和 `references/`。在新会话中使用 `$photo-skill` 调用。

## 使用示例

```text
使用 $photo-skill，生成一张自然窗光的半身人像，保留真实皮肤纹理。
```

```text
使用 $photo-skill，编辑这张照片，只把光线改成左侧柔和窗光，保持人物身份、服装、姿势和构图。
```

```text
使用 $photo-skill，为这件产品写一份可直接用于 image 模型的商业摄影提示词。
```

技能由宿主助手读取并调用其可用图像工具；只要求提示词时不会自动生图。技能文件本身不能让图像模型自行执行工具。

## 内容与来源

`SKILL.md` 是技能入口，`agents/openai.yaml` 是界面元数据，`references/` 包含摄影决策、人物与光线、图像工作流、检查清单及来源记录。

本次资料依据为用户提供的摄影教程图文包；公开目录、课程介绍、摘要与原创练习的范围记录在 `references/tutorial-pack.md`。既有扩展资料的来源线索见 `references/sources.md`。未收录付费课程全文或完整视频，不将目录介绍当作课程内容。
