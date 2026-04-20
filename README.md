# My Hexo Blog

这是一个使用 Hexo 框架和 Klise-enhanced 主题搭建的个人博客。

## 功能特点

- **现代化主题**：使用 Klise-enhanced 主题，支持响应式布局和深色模式
- **Markdown 支持**：使用 Hexo 内置的 Markdown 渲染器，支持丰富的 Markdown 语法
- **字数统计**：集成 hexo-wordcount 插件，显示文章字数和预计阅读时间
- **标签和分类**：支持文章标签和分类管理
- **自定义配置**：通过配置文件可以轻松自定义博客设置

## 技术栈

- **框架**：Hexo v7+
- **主题**：hexo-theme-Klise-enhanced
- **插件**：hexo-wordcount
- **部署**：可部署到 GitHub Pages、Vercel 等平台

## 快速开始

### 安装依赖

```bash
npm install
```

### 本地开发

```bash
hexo server
```

访问 http://localhost:4000 查看博客效果。

### 构建生产版本

```bash
hexo clean && hexo generate
```

构建后的文件会生成在 `public` 目录中。

## 主题配置

主题配置文件位于 `_config.hexo-theme-Klise-enhanced.yml`，可以根据需要修改以下设置：

- 网站标题、副标题和描述
- 导航菜单
- 社交链接
- 评论系统（支持 Valine、Waline 等）
- 自定义背景

## 目录结构

```
├── _config.yml          # Hexo 主配置文件
├── _config.hexo-theme-Klise-enhanced.yml  # 主题配置文件
├── source/              # 源代码目录
│   ├── _posts/          # 文章目录
│   └── ...
├── themes/              # 主题目录
│   └── hexo-theme-Klise-enhanced/  # Klise-enhanced 主题
├── node_modules/        # 依赖包
└── package.json         # 项目配置文件
```

## 写文章

使用以下命令创建新文章：

```bash
hexo new "文章标题"
```

文章会生成在 `source/_posts/` 目录中，使用 Markdown 格式编写。

## 部署

### GitHub Pages

1. 安装 hexo-deployer-git 插件：
   ```bash
   npm install hexo-deployer-git --save
   ```

2. 在 `_config.yml` 中配置部署信息：
   ```yaml
deploy:
  type: git
  repo: https://github.com/your-username/your-repo.git
  branch: gh-pages
   ```

3. 部署到 GitHub Pages：
   ```bash
   hexo deploy
   ```

## 主题特色

- **响应式设计**：适配桌面端、平板和移动设备
- **深色模式**：自动切换或手动切换
- **动态标题**：当页面失去焦点时，标签页标题会变化
- **自定义背景**：支持为明暗模式设置不同背景
- **插件兼容**：支持多种 Hexo 插件

## 许可证

MIT License
