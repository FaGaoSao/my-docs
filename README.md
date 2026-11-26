# my-docs

个人技术文档网站，使用 Markdown 编写、MkDocs Material 构建，通过 GitHub Actions 自动部署到 GitHub Pages。

## 项目简介

本仓库是「实践项目2：通过 GitHub Actions 自动部署静态文档到 GitHub Pages」的作业仓库。网站源码存放在 `docs/` 目录，构建配置为 `mkdocs.yml`，部署工作流为 `.github/workflows/deploy.yml`。

## 相关链接

- 网站地址：https://fagaosao.github.io/my-docs/
- 个人实验报告：[report/README.md](report/README.md)

## 本地预览

```bash
python -m venv .venv
.\.venv\Scripts\Activate.ps1
python -m pip install -r requirements.txt
python -m mkdocs serve
```

打开 http://127.0.0.1:8000/ 查看效果。构建检查使用 `python -m mkdocs build --strict`。

## 目录结构

```
my-docs/
├── .github/workflows/deploy.yml   # 自动构建与部署工作流
├── docs/                          # 网站源内容（4 个页面）
├── report/                        # 个人实验报告与截图
├── mkdocs.yml                     # MkDocs 配置
├── requirements.txt               # 依赖版本范围
└── .gitignore                     # 忽略 site/ 与 .venv/
```
