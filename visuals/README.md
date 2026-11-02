# 赛博神仙视觉素材

`material-scene.png`：2026-11-02 使用内置 image_gen 根据用户指定的原四张素材生成的纸石纹理、几何色块与星盘背景。原始文件 `exec-aa8aeb94-5a32-41ca-868f-71da85969a6f.png`，2171×724。提示要求：横向 3:1；左侧暖象牙白留字区、右侧墨绿矿物面与细黄铜星轨，少量朱红／赭石边角，下沿渐淡；无文字、控件、宫殿或玻璃建筑。背景只作装饰，不参与占卜计算。`symbols-v2.png` 四体系原图保持不变。

第二版图鉴插画位于 `illustrations-v2/`：`tarot-major.png` 为 6×4 格（前 22 格），`tarot-wands/cups/swords/pentacles.png` 分别为 4×4 格（前 14 格），`star-major/minor.png` 各为 4×4 格（前 14 格）。共覆盖 78 张牌及 28 颗星，备用格不展示。完整原图通过内置 image_gen 生成并复制保留，未裁切改写源文件；CSS 视窗按 `src/illustrations.ts` 的明确身份映射取图。所有原始提示词和生成文件来源见 `docs/visual-concepts/illustrations-v2/prompts.json`。

这些是 AI 辅助创作的现代抽象插画，不是历史牌面复刻或天文图；具体牌名、正逆位、星曜亮度与四化由界面真实数据标注，插画的物体数量不作为牌点、计算或解读依据。原有三种体系主题素材继续保留。

2026-11-02 使用内置 image_gen 生成。用户选择符号区分版为默认，并保留此前抽象人形、幻想人物两版，通过风格按钮切换。

- `symbols-v2.png`：四体系对照稿（六爻修正版）。塔罗扇形牌阵、周易六爻、八字四柱、紫微星宫。原始文件 `exec-aefa28e9-dfe3-4d59-aa35-20b38148da13.png`。
- `abstract-v1.png`：抽象人形与水墨主视觉，原始文件 `exec-f68f3690-a11f-4211-b585-e6d9e6ac676f.png`。
- `fantasy-v1.png`：幻想人物与观星殿主视觉，原始文件 `exec-af8b9110-9b36-4463-a731-0fbcbba8ca17.png`。

原图保留完整，`src/appearance.tsx` 用 CSS sprite 窗口仅展示插画区域。页面文本、表单和结果均由真实组件渲染，不展示原图中的示例文字或票数。体系插画是装饰身份图，不是实际抽牌或排盘依据；真实依据由原有 EvidenceView 独立呈现。

抽象人形的首页、结果页样稿和提示词见 `docs/visual-concepts/2026-11-02-abstract-v1/`；最新版提示词见 `docs/visual-concepts/identities-v2.md`。
