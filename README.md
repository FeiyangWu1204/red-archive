# The Red Archive · 私人档案室

Feiyang Wu 的互动个人网站。Three.js 复古书桌、雨夜窗景、EVA 海报，以及可装入播放器的四卷档案录像带。

在线访问：https://feiyangwu1204.github.io/red-archive/

## 本地运行

无需安装前端依赖。在项目根目录运行：

```sh
python3 -m http.server 8765 --directory dist
```

然后打开 http://localhost:8765/ 。请使用 HTTP 服务，直接双击 HTML 无法正常加载 ES modules 与模型。

## 内容与样式

- `dist/index.html`：页面结构、顶部个人资料内容和字体引用。
- `dist/archive.js`：展开阅读页的个人资料与作品文字。
- `dist/archive.css`：导航、按钮与阅读页样式。
- `dist/scene/channels/`：四卷录像带的内容、外壳配色与标签。
- `dist/scene/desktop.js`：3D 场景、录像带动作、海报和画面处理。
- `dist/scene/notepad/notepad.js`：弹出笔记的排版、字体和贴图。
- `dist/scene/tex/loading-room-v5.jpg`：与当前书桌对应的加载底图；修改海报或桌面陈设后需要重新生成。

## 部署

GitHub Pages 从 `codex/github-pages` 分支的根目录发布；`main` 分支保留开发源码，其中 `dist/` 是完整的静态网站目录。模型、贴图及音效均随目录提供；字体使用 Google Fonts，加载字体需要网络。

## 素材来源

场景改编自 Felix Rieseberg 的个人网站。原始模型、音效及图片的署名保留在页面与 `SOURCE-CREDITS.md` 中。本仓库没有为第三方素材授予新的许可。
