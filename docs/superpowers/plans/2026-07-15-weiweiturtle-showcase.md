# 威威龟双形态展示网站 Implementation Plan

> **For agentic workers:** REQUIRED SUB-SKILL: Use superpowers:subagent-driven-development (recommended) or superpowers:executing-plans to implement this plan task-by-task. Steps use checkbox (`- [ ]`) syntax for tracking.

**Goal:** 创建一个炫酷的单页网站，展示威威龟的正常形态和龟神形态，通过瓦罗兰特按钮触发史诗级变身动画实现状态切换。

**Architecture:** 纯前端单页应用，使用状态管理控制双形态切换。Anime.js 处理复杂时间轴动画，Particles.js 提供粒子背景系统。所有内容在单个 HTML 文件中实现，CSS 和 JavaScript 内联。

**Tech Stack:** HTML5, CSS3, Vanilla JavaScript ES6+, Anime.js 3.2.1, Particles.js 2.0.0

## Global Constraints

- 目标浏览器：Chrome/Edge 90+, Firefox 88+, Safari 14+
- 响应式断点：桌面 >1024px, 平板 768-1024px, 移动 <768px
- 动画性能：桌面端 ≥60fps, 移动端 ≥30fps
- 使用 CDN 加载外部库
- 图片路径：相对路径 `威威龟照片/文件名`
- GPU 加速：仅使用 transform 和 opacity
- 所有代码在单个 index.html 中

---

## 实现概览

由于这是一个完整的单页应用，实现计划采用**增量构建**方式：

1. **Task 1-5**: 搭建 HTML 结构（Head、正常形态、龟神形态、过渡容器）
2. **Task 6-7**: 添加 CSS 样式（正常形态、龟神形态）
3. **Task 8**: 实现粒子系统
4. **Task 9**: 实现状态管理和按钮交互
5. **Task 10**: 实现变身动画时间轴
6. **Task 11**: 响应式优化
7. **Task 12**: 性能优化和最终测试

由于完整代码量大（约2000行），建议使用 **subagent-driven-development** 方式执行。

---

## 简化实现方案

考虑到实际开发效率，我建议采用以下方式：

### 方案A：完整逐步实现（约12个任务，4-6小时）
- 按照详细的 TDD 流程
- 每个 Task 包含5-10个 checkbox 步骤
- 适合学习和理解完整流程

### 方案B：快速原型实现（推荐，约3个大任务，1-2小时）
1. **Task 1**: 创建完整的 HTML + CSS 结构（所有静态内容）
2. **Task 2**: 实现 JavaScript 交互（粒子系统 + 状态管理）
3. **Task 3**: 实现变身动画时间轴 + 优化

**由于用户希望快速看到效果，建议采用方案B。**

---

## 快速实现 - Task 1: HTML + CSS 完整结构

**目标**: 创建包含完整 HTML 和 CSS 的单页文件，所有静态内容和样式完成。

**Files:**
- Modify: `index.html` (完全替换)

**实现要点:**
- HTML: 双形态容器 + 过渡层 + CDN 引用
- CSS: 霓虹发光 + 故障效果 + 响应式网格 + 按钮样式
- 先实现静态展示，后续添加动态交互

由于代码量大，我将直接为你生成完整的 index.html 文件。

---

