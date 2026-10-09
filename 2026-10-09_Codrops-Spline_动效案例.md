# Codrops / Spline 动效案例学习

- **记录日期：** 2026-10-09
- **调研分工：** GPT-5.6 Terra Max 调研；主协调整合到训练库。
- **证据限制：** Codrops 教程和 demo 页面可打开但本轮没有实际滚动页面；Spline Community 页面可打开但本轮没有在场景画布里执行 hover。以下不声称真实交互已复测。

## Codrops：SVG mask 让滚动转场承担叙事

- [作者教程](https://tympanus.net/codrops/2026/03/11/svg-mask-transitions-on-scroll-with-gsap-and-scrolltrigger/)
- [直达 Demo](https://tympanus.net/Tutorials/SVGMaskScrollTransition/)
- **页面可见：** Demo 标出 `Scroll down`、FIRST/SECOND/THIRD IMAGE；教程说明用 GSAP、ScrollTrigger 与 SVG mask 构造四类全屏图像转场，包括横向/纵向百叶和随机栅格。
- **实现启发：** 触发器不是“进场一下”而是滚动进度；遮罩开启的先后、方向、网格密度与当前文字状态共同构成镜头顺序。教程也提到按屏幕比例重算 SVG 画布与格子。
- **设计判断：** 有价值的是场景切换与内容层级同步。作品展示可以先建立主图，再让一层遮罩揭开下一段；不应为了炫技把所有照片都加转场。
- **待复测：** 实际滚动时间线、触屏滚动表现、低性能设备下帧率与 prefers-reduced-motion 路径。
- **复用边界：** 代码文章可作学习来源；正式发布重建时用自制图片、版式与文案，不直接复制 demo 的素材或视觉编排。

## Spline Community：Boxes Hover

- [社区作品页](https://community.spline.design/file/a1f156f7-ef01-42d1-bf7b-5be1b7967b0a)
- [Spline Mouse Hover Event 文档](https://docs.spline.design/interaction-states-events-and-actions/events/mouse-hover-event)
- [Spline 场景优化文档](https://docs.spline.design/exporting-your-scene/how-to-optimize-your-scene)
- **可观察信息：** 社区页标题为 `Boxes Hover`，页头标示 Made in Spline 与 CC BY 4.0；本轮网页结果没有显示足够场景预览来确认具体悬停路径。
- **官方能力：** Spline 文档说 Mouse Hover Event 在物体被悬停时触发，并可连接 Transition、Animation、Particle Control、Create/Destroy Object、Switch Camera 等动作；鼠标离开后效果回到原状态。
- **设计判断：** hover 可以是局部状态生成器：它只改变被指向物体，而不是让场景一直自转。移动端需要点击/触摸或内容静态可读的替代状态。
- **授权边界：** 社区页标出的 CC BY 4.0 不自动证明场景中的每项模型、纹理或商标都按同一授权可复用；优先重建交互机制，使用自行制作的物件和素材。
- **待复测：** 在 Spline 场景画布中实际 hover，记录入场、离开复位和移动端替代行为。

## 小红书表达方式

这两个案例适合的共同讲法是“先给输入，再展示改变”：画面 A 写清滚动或 hover，画面 B 标出可见状态，再拆解素材/层级/时序。结尾给读者的是可重建的规则和自己的提示词，而非源站素材包。记录本次只完成页面级检查；要录屏前须另做交互复测。
