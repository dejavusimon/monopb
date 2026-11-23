# Mono PB 账务台（网页）

Mono Photobooth 内部用的活动、排班和账务网页。

这个仓库只放网页本身（`index.html`、图标、`manifest.webmanifest`），由 GitHub Pages 发布。

- **源代码里没有任何账目、成员或客户数据。** 打开网页只看到登录框，输对团队口令后，数据才会从后台读进来。
- **后台和数据不在这里。** 后台是一个 Google Apps Script 网页应用，数据存在 Google Sheet 里，代码放在另一个私有仓库。
- **后台网址写在 `index.html` 的 `API_URL` 里。** 这个网址公开也没关系：后台每次都会检查团队口令，口令连续输错太多次还会暂停 10 分钟。

## 不要提交

- 团队口令
- Google Sheet 的网址或 ID
- 任何账目、成员或客户的数据

## 更新网页

改好 `index.html` 后提交到 `main`。GitHub Pages 大约 1 分钟后会自动更新。
