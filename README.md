# 钳工理论考核练习系统

纯前端 PWA 练习系统，支持题库浏览、随机练习、评分、错题本、练习记录和离线缓存。

## 本地预览

```bash
python -m http.server 8000
```

然后打开：

```text
http://localhost:8000/
```

## GitHub Pages 部署

1. 在 GitHub 创建一个空仓库。
2. 在本目录执行：

```bash
git init
git add index.html styles.css app.js question_bank.js manifest.webmanifest service-worker.js icon.svg README.md .gitignore
git commit -m "Initial PWA quiz app"
git branch -M main
git remote add origin <你的仓库地址>
git push -u origin main
```

3. 进入 GitHub 仓库：Settings → Pages。
4. Source 选择 `Deploy from a branch`。
5. Branch 选择 `main`，目录选择 `/ (root)`。
6. 保存后等待部署完成。

访问地址通常是：

```text
https://<你的用户名>.github.io/<仓库名>/
```

## 手机添加到桌面

部署到 GitHub Pages 后，用手机 Chrome / Edge / Safari 打开 HTTPS 地址：

- Android Chrome/Edge：菜单 → 添加到主屏幕 / 安装应用
- iPhone Safari：分享按钮 → 添加到主屏幕

首次打开后会缓存离线资源，后续可离线使用。
