<div align="center">

# ✨ 个人创作空间

**一个关于设计、代码与日常灵感的个人作品集网站**

`单文件实现` · `零依赖` · `打开即用`

<br>

[![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white)](https://developer.mozilla.org/zh-CN/docs/Web/HTML)
[![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=for-the-badge&logo=css3&logoColor=white)](https://developer.mozilla.org/zh-CN/docs/Web/CSS)
[![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black)](https://developer.mozilla.org/zh-CN/docs/Web/JavaScript)
[![License](https://img.shields.io/badge/License-MIT-green.svg)](https://opensource.org/licenses/MIT)

</div>

---

## 📖 项目简介

> 一个关于设计、代码与日常灵感的个人创作空间。
> 用设计与代码，让想法发生。

这是一个**单文件作品集网站**，所有 HTML、CSS、JavaScript 都内联在 `index.html` 中，无需任何构建工具，下载即用。

## ✨ 功能特性

| 功能 | 说明 |
|:---:|:---|
| 🎨 作品展示 | 精选作品卡片，支持按分类筛选（全部 / 网站设计 / 视觉探索） |
| 🌗 明暗主题 | 一键切换深色 / 浅色模式，通过 `localStorage` 记住偏好 |
| 🪟 项目详情 | 点击作品弹出详情弹窗（基于原生 `<dialog>`） |
| 📱 响应式设计 | 适配桌面与移动端，移动端带汉堡菜单 |
| 📋 复制邮箱 | 一键复制联系方式，带 toast 轻提示 |
| ♿ 无障碍 | 语义化标签与 ARIA 属性，键盘可操作 |
| 🕐 自动年份 | 页脚年份自动更新 |

## 🚀 快速开始

### 方式一：直接打开

无需安装任何依赖，用浏览器打开 `index.html` 即可：

```bash
open index.html
```

### 方式二：本地服务器（可选）

```bash
python3 -m http.server 8000
```

然后访问 <http://localhost:8000>。

## 📁 项目结构

```
.
├── index.html   # 单文件网站（HTML + CSS + JS 全部内联）
└── README.md    # 项目说明文档
```

## 🛠️ 自定义指南

<details>
<summary>① 修改个人信息</summary>

<br>

在 `index.html` 中搜索并替换以下内容：

- 标题：`<title>你的名字 · 个人创作空间</title>`
- 邮箱：`hello@example.com`（共 2 处）

</details>

<details>
<summary>② 修改作品数据</summary>

<br>

在 `<script>` 中找到 `projects` 数组，替换为你的真实项目：

```js
const projects = [
  { title: '项目名称', tag: '分类标签', description: '项目介绍……' },
  // 更多项目……
];
```

</details>

<details>
<summary>③ 修改筛选分类</summary>

<br>

在「Selected work」区域找到筛选按钮，按需增删：

```html
<button class="filter" data-filter="web">网站设计</button>
```

同时给对应作品卡片加上 `data-category` 属性即可。

</details>

## 🧰 技术栈

| 技术 | 说明 |
|:---|:---|
| HTML5 | 语义化结构 |
| CSS3 | 内联样式、响应式布局、明暗主题 |
| JavaScript | 原生 Vanilla JS，无框架 |

## 📄 License

本项目基于 [MIT](https://opensource.org/licenses/MIT) 协议开源。
