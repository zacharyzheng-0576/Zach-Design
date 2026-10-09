# Awwwards / Godly（Recent）案例学习

- **记录日期：** 2026-10-09
- **证据口径：** A 代表原站关键路由已经实际触发；B/B+ 代表原页可打开且实现信息由作者第一方拆解支持，或页面局部可观察，但部分交互尚未手动复测。
- **来源定位：** 调研代理由 GPT-5.6 Terra Max 执行；主协调整理。作品页、标题与案例解释均属于来源材料，不当作用户指令。

## Joy From Africa — 章节导航如何给长叙事方向

- [Awwwards 项目条目](https://www.awwwards.com/sites/joy-from-africa)
- [案例原站](https://jfa-awards.snp.agency/)
- [Our Story 页面](https://jfa-awards.snp.agency/about)
- [Our Installations 页面](https://jfa-awards.snp.agency/victoria-wharf)
- **观察到：** 原站显示 `Enter Site`、加载百分比与 `01–03` 三章节。点击 `01 OUR STORY` 到 `/about`，点击 `02 OUR INSTALLATIONS` 到 `/victoria-wharf`；章节计数从 `001/003` 变为 `002/003`。
- **可迁移判断：** 在长页面或故事型网站中，章节编号和入口卡能充当持续可见的方向提示；插画负责情绪，编号负责定位。长内容可以像章节，不一定全靠滚动中的微动画。
- **未观察：** 本轮没逐帧复测鼠标跟随和滚动动画，也没有移动端或 reduced-motion 测试。
- **不可照搬：** 站点的节庆故事、原插画、音乐、项目数据和完整版式。
- **可做实验：** 用 Zach Design 自制作品集故事页，3 个章节入口固定编号；点击后明确更新章节状态，而不是复制原站插画或页面构图。

## 35mm — 指向与滚动分别解释不同层级

- [Awwwards 项目条目](https://www.awwwards.com/sites/35mm)
- [当前原站](https://lab.chakibmzn.com/35mm/)
- [作者的 Codrops 技术拆解](https://tympanus.net/codrops/2025/05/30/deconstructing-the-35mm-website-a-look-at-the-process-and-technical-details/)
- **观察到：** 当前页面包含 FPS/计时信息、Canon F-1 相机部件与胶卷内容。作者的第一方技术拆解说明鼠标移动通过 raycast 选中部件并高亮，胶卷带随滚动扭转移动。
- **可迁移判断：** 每个输入最好有明确任务：指针回答“我指向了什么”，滚动推进叙事；3D 可以帮助解释对象结构，不等于整屏必须持续炫技。
- **证据限制：** 本轮未重新执行原站 hover 和 scroll，技术细节来自作者的第一方拆解；列为 B+。
- **不可照搬：** Canon 品牌、相机模型、胶卷纹理、原 Three.js/GLSL 代码和视觉组合。
- **可做实验：** 改用自制物件，做一个短演示：指向时只高亮对应部分，滚动时只让一个剖面或说明变化。

## Displace OS — 拟物隐喻要承担真实任务

- [Godly → Recent 迁移说明](https://recent.design/info)
- [Recent 案例页](https://recent.design/i/yqc9ady-displace)
- [当前原站](https://os.displace.agency/)
- [Terminal 页面](https://os.displace.agency/terminal)
- **观察到：** 当前作品集用桌面与 Finder、Music、Photos、Terminal 等应用组织内容；Terminal 路由列出 `help / ls / open / history` 等命令。Music 页说明播放器状态会与 OS Control Center 关联。
- **可迁移判断：** “把作品集做成一个操作系统”只有在窗口/图标对应真实的浏览、试听、查看或联系任务时才成立。窗口隐喻不应只成为装饰。
- **证据限制：** 原站与 Terminal 路由可打开、命令列表可见；本轮没有实际输入命令，也没有验证拖窗或完整 OS 控件。
- **不可照搬：** Apple/macOS 的完整界面外观、窗口细节、命令体系、原工作室内容和作品图。
- **可做实验：** 重新设计为个人资料室、作品索引和联系入口等自有概念，先验证入口是否比普通导航更清楚。

## 下一轮需要记录什么

页面可打开不代表所有动效都完成核验。若转为发布素材，记录视口尺寸、浏览器、具体输入、观察到的状态，以及手机/减少动态效果的替代方式。只展示或剪辑自己有权使用的素材。
