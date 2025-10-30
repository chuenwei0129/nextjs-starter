# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## 项目概述

这是一个使用 Next.js 16 App Router、React 19 和 Tailwind CSS 4 的启动项目。

## 常用命令

### 开发与构建
- `npm run dev` - 启动开发服务器 (http://localhost:3000)
- `npm run build` - 构建生产版本
- `npm start` - 运行生产构建
- `npm run lint` - 运行 ESLint 检查

## 代码架构

### 项目结构
- **App Router**: 使用 Next.js 13+ 的 App Router (app/ 目录)
- **根布局**: `app/layout.tsx` - 定义全局 HTML 结构和字体配置
- **主页**: `app/page.tsx` - 应用入口页面
- **全局样式**: `app/globals.css` - Tailwind CSS 配置和全局样式

### 技术栈配置
- **TypeScript**: 启用严格模式，使用路径别名 `@/*` 指向根目录
- **字体**: 使用 Geist Sans 和 Geist Mono 字体，通过 `next/font/google` 自动优化
- **ESLint**: 使用 Next.js 推荐配置 (core-web-vitals 和 TypeScript 规则)
- **Tailwind CSS v4**: 通过 PostCSS 集成，支持暗色模式

### 开发注意事项
- 页面和组件使用 React Server Components (默认)
- 需要客户端交互时使用 `'use client'` 指令
- 图片优化使用 `next/image` 组件
- 暗色模式通过 Tailwind 的 `dark:` 前缀实现
