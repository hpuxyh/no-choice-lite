# 不做选择 Lite：简洁版

这是“简洁版”，代码和 Cloudflare Pages 项目都独立于游戏版。

| 版本 | 代码位置 | 线上地址 | 说明 |
| --- | --- | --- | --- |
| 简洁版 | `no-choice-lite/public/play.html` | https://no-choice-lite.pages.dev/play.html | 克制、工具化移动端样式。 |
| 游戏版 | `no-choice-demo/public/play.html` | https://no-choice.pages.dev/play.html | 像素/抽卡/模式卡片风格，对应“霸总模式 / AI 模式 / 玄学模式”。 |
| 原始版 | `no-choice-demo/src` 与 `no-choice-demo/index.html` | https://no-choice.pages.dev/ | React + Vite 原始 Web 原型。 |

核心交互、语音输入、定位、AI/POI 推荐和滑卡决策与游戏版保持一致，视觉层改为更克制的移动端工具风格。

## 本地运行

```bash
npm install
npm run dev
```

本地预览：

```text
http://127.0.0.1:5173/play.html
```

## 发布到 Cloudflare Pages

```bash
npm run deploy:pages
```

默认项目名：

```text
no-choice-lite
```

发布后的生产地址：

```text
https://no-choice-lite.pages.dev/play.html
```

## 说明

- `public/play.html` 是简洁版入口，不是游戏版。
- `public/minimal-theme.css` 是简洁版视觉覆盖层。
- 新站默认复用游戏版 `https://no-choice.pages.dev` 的 API，避免新 Cloudflare Pages 项目尚未配置密钥时推荐能力失效。
