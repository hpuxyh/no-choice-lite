# 不做选择 Lite

基于 `https://no-choice.pages.dev/play` 的简洁样式版本。核心交互、语音输入、定位、AI/POI 推荐和滑卡决策保持一致，视觉层改为更克制的移动端工具风格。

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
https://no-choice-lite.pages.dev/play
```

## 说明

- `public/play.html` 来自线上当前版本。
- `public/minimal-theme.css` 是简洁版视觉覆盖层。
- 新站默认复用 `https://no-choice.pages.dev` 的 API，避免新 Cloudflare Pages 项目尚未配置密钥时推荐能力失效。
