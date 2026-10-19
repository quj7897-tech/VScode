# 个人创作空间

一个关于设计、代码与日常灵感的个人作品集网站。单文件实现，无需构建工具，打开即用。

## ✨ 功能特性

- 🎨 **作品展示** — 精选作品卡片，支持按分类筛选（全部 / 网站设计 / 视觉探索）
- 🌗 **明暗主题** — 一键切换深色 / 浅色模式，并通过 `localStorage` 记住偏好
- 🪟 **项目详情弹窗** — 点击作品弹出详情（基于原生 `<dialog>`）
- 📱 **响应式设计** — 适配桌面与移动端，移动端带汉堡菜单
- 📋 **复制邮箱** — 一键复制联系方式，带 toast 提示
- ♿ **无障碍支持** — 语义化标签与 ARIA 属性
- 🕐 **自动年份** — 页脚年份自动更新

## 🚀 快速开始

无需安装任何依赖，直接用浏览器打开 `index.html` 即可。

```bash
# 方式一：直接打开
open index.html

# 方式二：用本地服务器（可选）
python3 -m http.server 8000
# 然后访问 http://localhost:8000
```

## 📁 项目结构

```
.
└── index.html   # 单文件网站（HTML + CSS + JavaScript 全部内联）
```

## 🛠️ 自定义指南

### 1. 修改个人信息

在 `index.html` 中搜索并替换以下内容：

- 标题：`<title>你的名字 · 个人创作空间</title>`
- 邮箱：`hello@example.com`（共 2 处）

### 2. 修改作品数据

在 `<script>` 中找到 `projects` 数组，替换为你的真实项目：

```js
const projects = [
  {title:'项目名称', tag:'分类标签', description:'项目介绍……'},
  // 更多项目……
];
```

### 3. 修改筛选分类

在「Selected work」区域，找到筛选按钮，按需增删：

```html
<button class="filter" data-filter="web">网站设计</button>
```

同时给对应的作品卡片加上 `data-category` 属性即可。

## 🧰 技术栈

- 纯原生 HTML5 + CSS3 + Vanilla JavaScript
- 无框架、无依赖、无构建步骤

## 📄 License

MIT
