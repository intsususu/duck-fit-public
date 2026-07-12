# duck-fit-public

AnewSpan 公开站点（GitHub Pages），用于托管 App Store Connect 与 App 内引用的公开页面。仓库名与 URL 中的 `duck-fit-public` 为沿用的托管路径，不作为对外产品名。

## 内容

- `index.html` — 站点落地页
- `privacy/` — 隐私政策三语页面
  - `index.html`（重定向到 `en.html`，作 ASC 默认英文 URL）
  - `en.html` / `zh-Hans.html` / `zh-Hant.html`

## 访问地址

GitHub Pages：`https://intsususu.github.io/duck-fit-public/`

- 落地页：`https://intsususu.github.io/duck-fit-public/`
- 隐私政策（英文，默认）：`https://intsususu.github.io/duck-fit-public/privacy/` 或 `…/privacy/en.html`
- 简中：`…/privacy/zh-Hans.html`
- 繁中：`…/privacy/zh-Hant.html`

## 与主仓库的关系

隐私政策内容源在主仓库 `duck-fit/docs/legal/privacy-policy.*.md` 与 `duck-fit/docs/site/privacy/*.html`。更新时同步本仓库对应文件并重新提交推送，GitHub Pages 会自动构建发布。

App 代码内 `PrivacyPolicy.baseURL`（`duck-fit/HealthApp/Features/Profile/ProfileSettingsViews.swift`）指向本站 `…/privacy/`。
