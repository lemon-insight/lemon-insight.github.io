# lemon-insight.github.io

本仓库是 **Lemon Insight** 博客的部署仓库，由 Hexo 自动生成并推送，用于 GitHub Pages 托管。

**请勿手动修改本仓库** —— 每次 `hexo d` 部署都会完全覆盖这里的内容。

- 线上地址：https://lemon-insight.github.io
- 源码仓库（写作与配置都在这里）：https://github.com/lemon-insight/blog-source

## 仓库内容说明

本仓库所有文件均由 Hexo 根据源码生成：

| 文件 / 目录 | 内容 |
|---|---|
| `index.html` | 网站首页 |
| `404.html` | 404 错误页 |
| `archives/` | 文章归档页（按年/月组织） |
| `2026/` 等年份目录 | 生成的文章页面，URL 格式为 `年/月/日/标题/` |
| `about/` | 关于页 |
| `tags/` | 标签页 |
| `categories/` | 分类页 |
| `friends/` | 友情链接页 |
| `masonry/` | 瀑布流页面的数据文件 |
| `css/` | 样式文件（主题样式、代码高亮、Tailwind 等） |
| `js/` | 脚本文件（主题功能、Typed 轮播、anime.js 开场动画、访问统计等） |
| `images/` | 头像、横幅图、favicon 等图片资源 |
| `fonts/` / `webfonts/` | 字体文件（Chillax、Geist、Font Awesome 图标字体等） |
| `assets/` | 主题附加资源 |

## 技术栈

- [Hexo](https://hexo.io/) 7.x — 静态站点生成器
- [hexo-theme-redefine](https://github.com/EvanNotFound/hexo-theme-redefine) 2.9.0 — 主题
- GitHub Pages — 托管

## 如何更新网站

所有修改都在源码仓库进行：

```bash
cd blog-source            # 进入源码仓库
hexo new "文章标题"        # 新建文章
hexo clean && hexo g      # 生成静态文件
hexo d                    # 部署（自动推送到本仓库）
```

部署后 GitHub Pages 会在 1-2 分钟内完成构建并上线。
