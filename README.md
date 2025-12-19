# Vitesse-Electron

一个基于 Electron + Vue 3 + Vite 的现代化桌面应用程序。

## 技术栈

- [Electron](https://www.electronjs.org/) - 跨平台桌面应用框架
- [Vue 3](https://v3.vuejs.org/) - 渐进式 JavaScript 框架
- [Vite](https://vitejs.dev/) - 下一代前端构建工具
- [TypeScript](https://www.typescriptlang.org/) - JavaScript 的超集
- [Pinia](https://pinia.vuejs.org/) - 状态管理
- [UnoCSS](https://uno.antfu.me/) - 原子化 CSS 引擎
- [Vue Router](https://router.vuejs.org/) - 官方路由
- [VueUse](https://vueuse.org/) - Vue 组合式工具集

## 环境要求

- Node.js >= 20.0.0 || >= 22.0.0 || >= 24.0.0
- pnpm

## 快速开始

### 安装依赖

```bash
pnpm install
```

### 开发模式

```bash
# 启动 Electron 开发环境
pnpm electron:dev
```

### 构建项目

```bash
# 构建 Electron 应用
pnpm electron:build

# 打包为可分发的应用程序
pnpm electron:pack

# 仅构建（不打包）用于测试
pnpm electron:preview
```

### 其他命令

```bash
# TypeScript 类型检查
pnpm type-check

# 代码格式化
pnpm format

# ESLint 检查并自动修复
pnpm lint
```

## 项目结构

```
.
├── electron/          # Electron 主进程和预加载脚本
│   ├── main.ts       # Electron 主进程
│   └── preload.ts    # 预加载脚本
├── src/              # 渲染进程（Vue 应用）
│   ├── manager/      # 管理模块
│   ├── pages/        # 页面组件
│   ├── router/       # 路由配置
│   ├── stores/       # Pinia 状态管理
│   ├── styles/       # 全局样式
│   ├── App.vue       # 根组件
│   ├── main.ts       # 应用入口
│   └── electron.d.ts # Electron 类型定义
├── dist/             # 渲染进程构建输出
├── dist-electron/    # 主进程构建输出
└── package.json      # 项目配置
```

## 功能特点

1. 🖥️ Electron 桌面应用支持
2. ⚡️ Vite 快速热重载
3. 🎨 UnoCSS 原子化 CSS
4. 📦 TypeScript 全栈类型支持
5. 🗂️ 基于文件系统的路由
6. 🍍 Pinia 状态管理
7. 🔧 开箱即用的开发工具 (Vue DevTools)
8. 🎯 图标自动导入 (Iconify)
9. 🎉 Canvas Confetti 效果支持

## 平台支持

- ✅ Windows
- ✅ macOS
- ✅ Linux

## 许可证

MIT
