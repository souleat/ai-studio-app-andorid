# AI Studio App

> **文档用途**：AI Studio 移动端应用的主文档，包含项目概览、技术栈说明及开发指南。
> **面向对象**：项目开发者、维护人员。

本项目是一个基于 **Vue 3**、**TypeScript** 和 **Capacitor** 构建的高性能跨平台移动应用，致力于提供极致的 AI 交互体验。

---

## 🚀 技术栈

*   **核心框架**: [Vue 3](https://vuejs.org/) (Composition API + `<script setup>`)
*   **构建工具**: [Vite 7](https://vitejs.dev/)
*   **语言**: [TypeScript](https://www.typescriptlang.org/)
*   **UI 组件库**: [Vant 4](https://vant-ui.github.io/vant/) (移动端优化)
*   **状态管理**: [Pinia](https://pinia.vuejs.org/)
*   **跨平台支持**: [Capacitor](https://capacitorjs.com/) (支持 iOS/Android 打包)
*   **样式处理**: Less
*   **图表展示**: ECharts & ECharts-GL
*   **包管理器**: **pnpm** (推荐)

---

## 📦 项目初始化

本项目已从 npm 迁移至 **pnpm**，以获得更快的速度和更小的磁盘占用。

### 前置要求
*   [Node.js](https://nodejs.org/) (建议 v20+)
*   安装 pnpm: `npm install -g pnpm`

### 安装依赖
```bash
pnpm install
```

---

## 🛠️ 开发与构建

### 启动测试服务器
```bash
pnpm run dev
```
启动后访问: `http://localhost:5173/`

### 项目打包
```bash
pnpm run build
```

### 预览构建产物
```bash
pnpm run preview
```

---

## 📂 项目结构规范

*   `src/components`: 通用组件
*   `src/views`: 页面视图
*   `src/store`: Pinia 状态管理
*   `src/assets`: 静态资源（图片、全局样式）
*   `public`: 公共静态资源
*   `capacitor.config.ts`: Capacitor 配置文件

---

## 📝 开发者备注

*   **依赖管理**: 强制使用 `pnpm`。避免直接使用 `npm install` 以免产生冗余的 `node_modules`。
*   **环境说明**: 
    *   `.env.development`: 开发环境配置
    *   `.env.production`: 生产环境配置
