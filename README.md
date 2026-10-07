# Gitty Age · GitHub 账号年龄查询

输入一个 GitHub 用户名，查看该账号注册了多久（精确到「几年几个月几天」），以及注册时间、公开仓库数、粉丝数。

**纯静态单文件网页**，无后端、无数据库、不需要任何 Token。数据来自 GitHub 官方公开 API（未登录额度 60 次/小时，个人使用足够）。

## 本地预览

直接双击 `index.html` 用浏览器打开即可。

## 部署到 GitHub Pages（免费托管）

1. 在 GitHub 新建一个仓库，例如 `gitty-age`
2. 把 `index.html` 推上去：
   ```bash
   git init
   git add .
   git commit -m "init: GitHub 账号年龄查询工具"
   git branch -M main
   git remote add origin https://github.com/你的用户名/gitty-age.git
   git push -u origin main
   ```
3. 打开仓库 **Settings → Pages**，Source 选 `Deploy from a branch`，Branch 选 `main` / `root`，保存
4. 等 1 分钟，访问 `https://你的用户名.github.io/gitty-age/` 即可

## 小技巧

URL 后面带 `?u=用户名` 可直接查询，例如：
`https://你的用户名.github.io/gitty-age/?u=torvalds`
