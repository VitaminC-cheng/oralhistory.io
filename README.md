# 如风如日，落地生根

霹雳华文独中复兴运动口述史研究展示网站。项目以静态网页形式整理研究背景、口述访谈、历史图像、文献材料、互动地图、数据看板和研究报告等内容。

## 项目内容

- `index.html`：网站首页，包含项目介绍、材料入口、研究报告入口和团队介绍。
- `interviews.html`：口述访谈内容与逐字稿入口。
- `photos.html`：采访照片与历史图像展示。
- `journal.html`：文献材料展示。
- `source.html`：选题背景材料。
- `map.html`：互动地图页面。
- `data-board.html`：数据看板页面。
- `article.html`：研究报告全文页面。
- `styles.css`：网站主要样式。
- `script.js`、`animation.js`：页面交互与动画脚本。
- `article-assets/`、`journal-assets/`、`source-assets/`、`pic/`、`pic-web/`：图片、档案和页面素材。

## 本地预览

这是一个纯静态网页项目，不需要安装依赖或执行构建步骤。进入项目目录后启动一个本地静态服务即可预览：

```bash
python -m http.server 8000
```

然后在浏览器打开：

```text
http://127.0.0.1:8000/index.html
```

如果系统中没有 `python` 命令，也可以使用任意静态文件服务器打开项目目录，例如 VS Code Live Server。

## 上传到 Git 仓库

首次上传时可以按下面流程操作：

```bash
git init
git add .
git commit -m "Initial static website"
git branch -M main
git remote add origin <你的仓库地址>
git push -u origin main
```

如果仓库已经初始化，只需要执行：

```bash
git add .
git commit -m "Update static website"
git push
```

## GitHub Pages 部署

如果要用 GitHub Pages 展示：

1. 将仓库上传到 GitHub。
2. 进入仓库的 Settings。
3. 打开 Pages 设置。
4. Source 选择 `Deploy from a branch`。
5. Branch 选择 `main`，目录选择 `/root`。
6. 保存后等待 GitHub 生成访问地址。

## 维护说明

- 上传前建议确认所有图片、字体和文档素材都已经放在项目目录内。
- 网页中的资源路径应尽量使用相对路径，例如 `./journal-assets/1.png`，避免使用本机绝对路径。
- `.gitignore` 已忽略系统缓存、编辑器配置、临时文件、依赖目录和本地助手工作目录，不会忽略网页源码、图片、字体、Markdown、Word 文档等项目内容。
