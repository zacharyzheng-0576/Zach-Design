# 03 Dennis · 页尾轻磁吸按钮

本期名称：**轻磁吸按钮**。已完成原站 Live Photo 录制与配对检查，并整理一份可独立复制的完整复刻提示词；网页实现、提示词图和平台发布尚未完成。

## 文件入口

| 文件 | 用途 |
| --- | --- |
| [Live Photo JPG](素材/live-photo/Zach-Design-03-Magnetic-Button.jpg) + [MOV](素材/live-photo/Zach-Design-03-Magnetic-Button.mov) | 一组 Live Photo，保留两者且保持配对 |
| [视频预览](素材/01-live-preview.mp4) | 查看动态；MP4 本身不是 Live Photo |
| [封面](素材/01-live-cover.png) | 与视频 1.5 秒位置对应 |
| [效果观察](内容/交互观察.md) | 触发、变化、原站机制与证据 |
| [复刻提示词](内容/复刻提示词.md) | 一句话解释和可直接复制的完整提示词 |
| [使用说明](素材/使用说明.txt) | 在照片中识别与传输的方法 |
| [反馈记录](反馈/反馈记录.md) | 记录意见、发布信息和复盘 |

## 复刻状态

提示词针对页尾邮箱 CTA，写明了轻量磁吸参数、填充方向、移动端边界和验收状态。当前只有原站实况与提示词；还没有运行提示词生成复现网页，因此不宣称实现完成或像素级通过。

## 录制与本地验证

- 来源：[Dennis Snellenberg 原站](https://dennissnellenberg.com/)，原站设计与开发 Dennis Snellenberg。
- 录制时间：`2026-10-09T10:22:40.061Z`；浏览器：`152.0.7977.84`。
- 浏览器视口与输出：810 × 1080，3:4；使用实际鼠标和滚轮输入，未改动网页 DOM、样式和原有动画。
- 全视口成片，无裁切、外框、字幕或人造动画。CDP 不包含系统鼠标图形，画面通过控件响应展示输入效果。
- 成片 3 秒、30 fps、90 帧，无音轨。保留 179 张变间隔源帧，不能把源帧数量当成成片帧率。
- [编码视频解码检查](素材/source/video-check/verification.json)：7 个时间位置均可解码，尺寸和时长符合预期。
- [Live Photo 本轮验证](素材/source/live-photo-verification.json)：图片与视频标识一致、含 1.5 秒静态时间标记，`PHLivePhoto.request` 接受。
- iPhone“照片”、AirDrop 和小红书实际导入播放尚未验证；本次没有访问或写入个人照片库。

## 终审与协作记录

GPT-6 Astra Ultra 终审：**通过**。邮箱按钮向左上与右下轻微移动，退色并归位；约16px×9px的变化，旁边电话按钮可作为固定参照。仅验证邮箱按钮。详见 [终审记录](素材/source/final-review.json)。

模型职责与本次实际安排统一见 [桌面 README](../../../README.md#协作分工)。GitHub 本次未操作。
