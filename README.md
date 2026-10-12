# HAOYANERIC.github.io

蒋昊延的个人主页，纯 HTML / CSS 单页，无任何构建工具和 JavaScript，由 [GitHub Pages](https://pages.github.com) 托管。

上线后的访问地址：<https://haoyaneric.github.io>

## 目录结构

```
├── index.html    # 页面内容（研究兴趣 / 教育背景 / 项目经历 / 技能 / 荣誉）
├── style.css     # 样式（极简学术风，强调色 --accent）
└── favicon.svg   # 网站图标
```

## 本地预览

任选一种：

```bash
python -m http.server 8000    # 访问 http://localhost:8000
# 或直接双击 index.html 用浏览器打开
```

## 如何修改内容

所有内容都在 `index.html` 里，结构与简历一致，直接编辑对应 `<section>` 即可：

- 头部：姓名、学院专业、联系方式
- `#interests`：研究兴趣
- `#education`：教育背景（学积分、课程）
- `#projects`：项目经历（每个项目一个 `<article class="entry">`）
- `#skills` / `#honors`：技能、荣誉

改样式调 `style.css` 顶部的 `:root` 变量（`--accent` 强调色、`--text` 正文色）。

## 发布上线

```bash
git add .
git commit -m "更新主页"
git push origin main
```

推送后约 1~2 分钟生效。首次使用请到 GitHub 仓库 **Settings → Pages** 确认 Source 为 `main` 分支 `/ (root)`。
