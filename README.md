# 客情宝 · 官方落地页

销售人员的客户记忆外挂 —— 微信小程序「客情宝」的官方引流落地页（单页静态站）。

## 内容
- `index.html`：单页落地页（移动优先，内联 CSS/JS，无外部框架依赖）
- `qrcode.png`：微信小程序码（建议替换为 mp 后台导出的高清原图）
- `.nojekyll`：关闭 GitHub Pages 的 Jekyll 处理，避免 `_` 前缀文件被忽略

## 本地预览
直接用浏览器打开 `index.html` 即可。

## 部署到 GitHub Pages
1. 在 GitHub 新建一个仓库（如 `keqingbao-landing`）
2. 把本目录内容推送到该仓库：
   ```bash
   git remote add origin https://github.com/<你的用户名>/<仓库名>.git
   git branch -M main
   git push -u origin main
   ```
3. 仓库 Settings → Pages → Source 选 `main` 分支 / `(root)` → Save
4. 几分钟后得到地址：`https://<你的用户名>.github.io/<仓库名>/`

## 自定义域名（可选）
在 Pages 设置里填自己的域名（如 `keqingbao.com`），并按提示在域名解析加 CNAME 记录。
注意：GitHub Pages 国内访问偶有不稳定，正式对国内 toC 投放建议搭配备案自有域名 + 国内托管。

## 同步更新
改完 `index.html` 后：
```bash
git add -A && git commit -m "更新落地页" && git push
```
