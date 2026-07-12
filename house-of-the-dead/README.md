# 死亡之屋 · 复刻版 — 第一章「馆」

向 1996 年 SEGA 街机经典《The House of the Dead》致敬的轨道光枪射击游戏。

**正式版**（`index.html`）：three.js + 写实风格恐怖角色。敌人阵容全部为
真实比例的骨骼动画模型（Sketchfab CC-BY）——**蹒跚尸**（rato biônico games，
含三种死法与方向受击）、**憔悴尸**（pxltiger，全 PBR 贴图夜光眼）、
**舔食者**（italianPie，低伏疾爬），Boss 为**苍白之物**——《SCP:
Containment Breach》的 SCP-096（CC-BY-SA），尖啸入场、弱点心脏。
四个场景（雨夜墓园/藏书馆/宴会厅/大圣堂）
使用 KayKit **Halloween Bits** 与 **Dungeon Remastered** CC0 资产包搭建
（墓碑/地穴/铁栅栏/南瓜灯/书墙/立柱/火把/军旗等道具）。
点光源 + 指数雾 + 640×360
低分辨率渲染 + 噪点扫描线后处理。模型经 gltf-transform 裁剪动画、
贴图压成 webp 后以 base64 内嵌，整个游戏仍是**单个 HTML 文件**，无需服务器。

历史版本同目录保留：`retro-3d.html`（纯手写 WebGL 引擎 + 程序化放样建模）、
`classic-2d.html`（Canvas 2D 版）。

恐怖氛围系统：全场景黑暗层 + 光池（月光/烛火/枪口焰会真实照亮黑暗），
丧尸从黑暗中浮现、远处只见发光的眼睛；蹒跚急停的步态与随机抽搐；
尸体和血迹永久留在地面；失谐低鸣 drone、不和谐音刺、灯光失灵、
闪电雷暴、手持镜头漂移，以及胶片噪点 + 扫描线 + 暗角的 CRT 后处理。

## 运行

直接用浏览器打开 `index.html`（3D 版）或 `classic-2d.html`（2D 版）即可，无需服务器。

## 操作

| 操作 | 按键 |
| --- | --- |
| 瞄准 | 鼠标移动 |
| 射击 | 鼠标左键 / 触屏点击 |
| 装弹（6 发弹匣） | `R` / 鼠标右键 / 右下角按钮 |
| 暂停 | `P` / `Esc` |
| 静音 | `M` |

## 玩法

- 一个完整章节：雨夜外庭大门 → 藏书馆 → 宴会大厅 → **大圣堂**（双层挑高
  哥特中殿：巨型玫瑰花窗、柱廊军旗、体积光柱——Boss 战就在花窗月光下）。
- **伏击链玩法**（核心循环）：没有一波波走来的怪。每个敌人都藏在场景里
  ——掘开的坟、棺材里、书架后、帷幕后、**你的身后**、甚至你留在地上的尸体——
  先从声音方位听到预警（3D 声像），镜头随即**猛甩过去**，它已经在向你
  狂奔：你只有 2~3 秒（逐幕收紧）爆头，失手就挨爪。击中身体可以击退
  **买 0.6 秒**再补枪；反应越快加分越高（0.9 秒内爆头 +300，连续快杀
  COMBO 递增）；起身瞬间击杀有「先发制人」奖励。准星上有红色倒计时环。
- 伏击序列每次游玩**随机抽取**：藏点、顺序、间隔都不同，二周目照样被吓；
  后期会出现**双重伏击**（两个方向几乎同时）。伏击之间是刻意的死寂——
  那是你唯一的装弹窗口。Boss 半血狂暴后也会从背后召唤伏击。
- 三幕搭建在同一条世界轴上，由石廊真实连通：清完一幕后镜头会推开铁门、
  穿过火把走廊一路走进下一幕（雾色与灯光沿途渐变），全程无切换黑屏。
- **电影化镜头**：出怪甩镜、平民入场跟拍、每波最后一杀慢动作处决镜头、
  Boss 亮心特写与击杀慢镜，配信箱黑边与 AMS 电台通讯字幕（打字机式）。
- **可互动场景**：油灯/油桶可以射爆（火球+范围杀伤）、南瓜灯可以打碎、
  木箱藏着生命、金柜藏着大分；标志性的**挟持营救**事件——僵尸抓住平民，
  在它撕咬前精准击毙（别打中人质！），救下可获生命奖励。
- 敌人：**蹒跚尸**（破土/翻窗突入，三种死法、按中弹方向受击）、
  **憔悴尸**（夜光眼写实僵尸，前倒/后倒两种倒地）、**舔食者**
  （低伏疾爬、飞身扑击，反应窗口最短），Boss 为**苍白之物**
  （SUBJECT: 096-B——尖啸暴走的苍白瘦长人形，狂暴后从背后召唤伏击）。
- 平民为真人模型（便装村民 / 白大褂研究员，随机出现），头顶绿色
  「平民」标记，被挟持时闪烁「人质」——和怪物一眼区分。
- **爆头**即死并有额外加分；子弹打空要及时装弹。
- **不要射击平民**——护送他们逃脱可以回复 1 点生命。
- Boss「苍白之物 THE PALE ONE」：弱点是胸口的**心脏**，蓄力攻击时集火可以打断它。
- 生命耗尽可以无限投币 CONTINUE（街机传统艺能），通关按命中率结算 S–D 评级。

## 素材致谢

- 敌人角色（均为 Sketchfab 作品，**CC-BY 4.0**，已按许可署名）：
  - 蹒跚尸：《zombie》by **rato biônico games**（sketchfab.com/felip32pppp）；
  - 憔悴尸：《Zombie》by **pxltiger**（sketchfab.com/pxltiger）；
  - 舔食者：《Zombie licker》by **italianPie**（sketchfab.com/italianPie）。
- Boss「苍白之物」：SCP-096 模型与动画取自 **《SCP – Containment Breach》**
  （Joonas Rikkonen "Regalis" 与 SCP:CB 团队，
  [github.com/Regalis11/scpcb](https://github.com/Regalis11/scpcb)），
  **CC-BY-SA 3.0** 许可——本作对该模型的裁剪/压缩版本依 ShareAlike
  条款同样以 CC-BY-SA 3.0 提供。
- 场景道具：**KayKit Halloween Bits** 与 **KayKit Dungeon Remastered**
  （[github.com/KayKit-Game-Assets](https://github.com/KayKit-Game-Assets)），Kay Lousberg 制作，CC0 许可。
- 平民角色：**Quaternius — Ultimate Animated Character Pack**
  （[quaternius.com](https://quaternius.com)），CC0 许可。
- 恐怖场景件（蛛网/掘开的坟/祭坛/烛堆/火盆）：**Quaternius 地牢包**（CC0）
  与 **Kenney — Graveyard Kit**（[kenney.nl](https://kenney.nl)，CC0）。
- 引擎：three.js（MIT）。其余贴图（含玫瑰花窗）、音效均为程序化生成。
