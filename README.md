# README

## 关于本站

这是一个用于存放本科学习笔记的个人网站。

## 技术栈

- [MkDocs](https://www.mkdocs.org/) - 静态站点生成器
- [Material for MkDocs](https://squidfunk.github.io/mkdocs-material/) - 主题
- [GitHub Pages](https://pages.github.com/) - 托管

## 项目结构

```
website/
├── mkdocs.yml          # 站点配置（导航/主题/插件/扩展）
├── pyproject.toml      # Python 依赖（mkdocs, mkdocs-material）
└── docs/
    ├── index.md        # 首页
    ├── about.md        # 关于页
    ├── stylesheets/    # 自定义 CSS
    ├── javascripts/    # MathJax 配置
    ├── math/           # 数学：信息论、数值分析
    ├── cs/             # 计算机科学：编译原理、软件基础
    └── ai/             # 人工智能
```

### 模块说明

- **配置 / 全局**
  - `mkdocs.yml`：定义左侧导航、主题色、Markdown 扩展，改它会影响**所有页面**的整体布局。
  - `docs/stylesheets/extra.css`：自定义样式，覆盖首页学科卡片（`.grid.cards`）、课程入口卡片（`.course-portal/.course-card`）和章节底部导航按钮（`.course-nav`）。
  - `docs/javascripts/mathjax.js`：启用 `\(...\)` / `\[...\]` 公式渲染，影响**所有含数学公式的页面**。

> 新增页面后，需要同步在 `mkdocs.yml` 的 `nav` 中登记，否则不会出现在导航栏中。

## 本地预览

```bash
uv sync
uv run mkdocs serve
```

## 联系方式

- GitHub: [Elena](https://github.com/ElenaGong)
