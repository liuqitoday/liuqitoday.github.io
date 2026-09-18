# 100067.xyz

Freddy 的身份主页。旧博客日期路径 301 到 [blog.100067.xyz](https://blog.100067.xyz)。

源码在 GitHub，站点由 **Cloudflare Pages** 发布（国内访问比 GitHub Pages 稳）。

## 部署

Cloudflare Dashboard → Workers & Pages → Create → Pages → Connect to Git：

- 仓库：`liuqitoday/liuqitoday.github.io`
- Framework preset：`None`
- Build command：留空
- Build output directory：`/`

自定义域名：

- `100067.xyz`
- `www.100067.xyz`（跳到 apex）

DNS 在 Cloudflare 本区，加上域名后会自动出橙云记录。不要再把 apex 指到 GitHub Pages 的 A 记录。

## 文件

- `_redirects`：Cloudflare Pages 的 301（日期路径、archives、tags、atom.xml）
- 同路径下的 `index.html`：给 `liuqitoday.github.io` 的 HTML 跳转兜底
- `CNAME`：GitHub Pages 仍会把 `liuqitoday.github.io` 指到 apex
