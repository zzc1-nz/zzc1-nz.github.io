# zzc1-nz.github.io

个人主页 —— 使用 GitHub Pages 托管。

**访问地址**：https://zzc1-nz.github.io

## 说明

- `index.html` —— 单文件静态主页（无构建步骤、无外部依赖，样式与脚本全部内联）
- 自适应深色 / 浅色主题（跟随系统 `prefers-color-scheme`）
- 响应式布局，适配手机与桌面

## 本地预览

直接双击 `index.html` 用浏览器打开即可；或起一个静态服务器：

```bash
python -m http.server 8000
# 然后访问 http://localhost:8000
```

## 如何修改

| 想改什么 | 改哪里 |
|---|---|
| 一句话简介 | `index.html` 中 `class="subtitle"` 那一行 |
| 关于我 | `<h2>关于我</h2>` 下面的段落 |
| 技术栈标签 | `<div class="tags">` 里的 `<span class="tag">` |
| 项目卡片 | `<div class="card">` 整块，可复制多份 |
| 配色 | `:root` 里的 CSS 变量（`--accent` 是主色） |

## 部署

推送到 `main` 分支即自动生效（GitHub Pages 默认从 `main` 分支根目录发布）。

```bash
git add .
git commit -m "update homepage"
git push
```
