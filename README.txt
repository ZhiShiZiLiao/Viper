VITRAIL · 圣书 — 交付说明
================================

【这是什么】
一个自包含的哥特风格单页网站。双击 index.html 即可本地打开，
或整个 dist 目录丢到任意静态服务器。

【文件结构】
  index.html          主页面（与 single.html 内容相同）
  assets/             图片与音乐（7 个）
    statue.png            天使雕塑
    mountain-wide.png     雪山背景
    bg-smoke.jpg          红黑烟雾底图
    cover-sanctuary.jpg   书一封面（教堂剪影）
    cover-hymn.jpg        书二封面（骨架玫瑰）
    cover-sleep.jpg       书三封面（烟雾窗）
    bgm.mp3               背景音乐
  vendor/             three.js（本地，非 CDN）
    three.module.js
    jsm/RoomEnvironment.js
    jsm/RoundedBoxGeometry.js

【联网依赖】
字体走 Google Fonts（Anton / Oswald / Noto Serif SC / Sora）。
离线打开时字体会回退到系统字体，页面功能不受影响，只是字形不同。
要完全离线，需把字体文件也下载进 assets 并改 @font-face。

【本地预览】
three.js 用 ES Module，部分浏览器用 file:// 直接双击可能因
跨域限制加载失败。推荐用任意静态服务器预览，例如：
  npx serve dist
  或 python -m http.server（在 dist 目录里）

【交互】
- 首页 → 点「聆听神祇」进书页
- 书页 → 拖动旋转书本，点书打开详情（书会自己飞过去，无黑屏转场）
- 详情页「点击跳转」→ 三本书各链接一个金山文档
- 右上角圆形按钮 / 键盘 M 键 → 开关背景音乐

生成日期：2026-11-22
