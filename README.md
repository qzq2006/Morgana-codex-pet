# Morgana Codex Pet

一个以《女神异闻录 5》摩尔加纳（Morgana）和人格面具 Zorro 为主题的 Codex 桌宠。

本项目使用 Codex Pet v2 图集格式，包含完整的基础状态动画、左右移动动画，以及 16 个观察方向。工作、审查和失败状态会出现 Zorro；其余状态保持 Morgana 的桌宠形象。

> 这是非官方的粉丝创作项目，与 Atlus、SEGA 或 OpenAI 无隶属或授权关系。相关角色及商标归各自权利人所有。

![完整动作图集预览](qa/contact-sheet-extended.png)

## 特点

- 更自然的左右跑步循环：触地、下压、蹬地、腾空相位完整，肩胯反向运动，围巾和尾巴延迟跟随。
- 左右跑步共用同一套规范步态（右向为逐帧水平镜像），因此两个方向的节奏与四肢配合完全一致。
- 更灵动的待机动作：呼吸、眨眼、轻微耳动，以及错相的尾巴和围巾摆动。
- 更有力量感的工作状态：Zorro 完成蓄力、剑击、回弹和收势，同时保持 Morgana 在前景清晰可辨。
- 跑步与待机帧的四肢结构统一：每帧恰好两条连接的手臂（各带白爪）与两条腿，没有游离的重复手爪碎片。
- 16 个观察方向，支持 Codex Pet v2 的方向响应。
- 最终图集已经过帧数、透明度、色键残留、尺寸和视觉连续性检查。

## 安装

仓库中的 `package` 目录就是可安装包。Windows PowerShell：

```powershell
$petDir = Join-Path $env:USERPROFILE ".codex\pets\morgana-zorro"
New-Item -ItemType Directory -Force -Path $petDir | Out-Null
Copy-Item -LiteralPath ".\package\pet.json" -Destination $petDir -Force
Copy-Item -LiteralPath ".\package\spritesheet.webp" -Destination $petDir -Force
```

随后在 Codex 中选择 `Morgana + Zorro`。如果 Codex 已经打开并缓存了旧图集，请切换一次桌宠或重启 Codex。

## 图集规格

| 项目 | 数值 |
| --- | --- |
| Sprite version | 2 |
| 图集尺寸 | 1536 × 2288 |
| 网格 | 8 列 × 11 行 |
| 单元格 | 192 × 208 |
| 运行时文件 | `package/spritesheet.webp` |

状态行映射：

| 行 | 状态 | 有效帧 | 用途 |
| ---: | --- | ---: | --- |
| 0 | `idle` | 6 | 待机、呼吸和眨眼 |
| 1 | `running-right` | 8 | 向右移动 |
| 2 | `running-left` | 8 | 向左移动 |
| 3 | `waving` | 4 | 挥手和吸引注意 |
| 4 | `jumping` | 5 | 跳跃 |
| 5 | `failed` | 8 | 失败、取消或阻塞反馈 |
| 6 | `waiting` | 6 | 等待确认或用户输入 |
| 7 | `running` | 6 | 正在执行任务；不是方向跑步 |
| 8 | `review` | 6 | 准备审查或展示结果 |
| 9 | `look-row-9` | 8 | 000°–157.5° 观察方向 |
| 10 | `look-row-10` | 8 | 180°–337.5° 观察方向 |

## 项目结构

```text
package/      可直接安装的 pet.json 和 spritesheet.webp
final/        最终 v2 图集、布局清单和结构验证结果
references/   用于确认角色身份的源参考图
qa/           最终联系表、动画预览和发布 QA 证据
pet_request.json  可移植的宠物规格与状态定义
```

仓库只保留最终发布与审计所需文件。生成提示词、横向生成条、拆分帧、8×9 中间图集和本地返修工作区不属于发布内容。

## 预览

常用动画可以在 `qa/previews` 中单独查看。预览 GIF 使用统一的 90 ms 帧间隔并无限循环，因此循环回到第一帧时不会有额外的停顿：

- [`idle.gif`](qa/previews/idle.gif)
- [`running-right.gif`](qa/previews/running-right.gif)
- [`running-left.gif`](qa/previews/running-left.gif)
- [`running.gif`](qa/previews/running.gif)
- [`waiting.gif`](qa/previews/waiting.gif)
- [`review.gif`](qa/previews/review.gif)

包含全部状态和观察方向的总览见 [`qa/contact-sheet-extended.png`](qa/contact-sheet-extended.png)。

## 验证状态

当前发布图集通过以下检查：

- 8 × 11、1536 × 2288 的 Codex Pet v2 结构校验。
- 所有必需状态帧存在，未使用的格子保持透明。
- 洋红色键像素与边缘污染均低于验证阈值，透明 RGB 残留为 0。
- 左右跑步、待机和工作循环通过独立逐帧视觉复核。
- 左右跑步行额外做了逐像素结构校验：每帧肢体白块恒为 4（两手两脚）、游离碎片为 0、轮廓连通块为 1、边缘像素为 0；循环各步的帧间相似度中，`7 → 0` 的接缝步相似度最高，即循环闭合最平滑。
- 第 0 行与第 3–10 行未受本次跑步修复影响，与上一版图集逐像素一致。
- `final/spritesheet-extended.webp` 与 `package/spritesheet.webp` 的 SHA-256 一致。

详细结果位于 [`qa/release-audit.json`](qa/release-audit.json)、[`qa/package-validation.json`](qa/package-validation.json)、[`qa/final-visual-qa.json`](qa/final-visual-qa.json) 和 [`qa/running-animation-fix.json`](qa/running-animation-fix.json)。

## 发布说明

当前仓库是最终发布版。安装时只需要复制 `package` 中的两个文件；`final` 和 `qa` 用于复核发布内容，不参与运行。
