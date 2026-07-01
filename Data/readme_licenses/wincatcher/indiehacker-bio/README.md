[English](README-EN.md) | [简体中文](README.md) | [繁體中文](README-Hant.md) | [日本語](README-JA.md)



# Indiehacker Bio

Indiehacker Bio 是一个现代化的、多语言支持的个人展示网站，专为独立开发者和互联网创业者设计。本项目使用 Next.js 构建，结合了多种先进的 Web 技术，为用户提供了一个优雅、响应式的在线个人简介平台。

## DEMO

[ https://biobio.top/zh/ ]( https://biobio.top/zh/ )

## 预览

![独立开发者在线社媒、项目展示开源模板-Indiehacker-bio-social-media-projects-theme-light](https://github.com/user-attachments/assets/d1107139-f019-4fe3-b2cd-9fb764e3e01d)

## 项目特色

1. **多语言支持**：支持英语、简体中文、繁体中文和日语，使用 next-intl 实现无缝的语言切换。

2. **响应式设计**：采用 Tailwind CSS 构建，确保在各种设备上都能完美展示。

3. **深色模式**：内置深色模式支持，提升用户体验。

4. **动画效果**：使用 Framer Motion 实现流畅的页面动画，增强视觉吸引力。

5. **模块化结构**：项目结构清晰，组件化设计便于维护和扩展。

6. **SEO 优化**：使用 Next.js 的元数据 API，优化搜索引擎表现。

7. **社交媒体集成**：展示多个社交媒体链接，方便访客快速了解和联系。

8. **项目展示**：独立的项目展示区域，突出个人成就。

9. **性能优化**：利用 Next.js 的图片优化和代码分割特性，提升加载速度。

10. **可定制性**：易于根据个人需求进行定制和扩展。

## 使用指南

### 安装

1. 克隆仓库：
   ```
   git clone https://github.com/wincatcher/indiehacker-bio.git
   ```

2. 安装依赖：
   ```
   cd indiehacker-bio
   npm install
   ```

### 配置

1. 语言设置：
   - 编辑 `src/i18n/routing.ts` 文件来配置支持的语言。
   - 在 `messages` 目录下添加或修改相应的语言文件。

2. 个人信息：
   - 修改 `src/data/socialLinks.ts` 来更新社交媒体链接。
   - 编辑 `src/data/projects.ts` 来展示您的项目。

3. 样式定制：
   - 主要样式在 `src/app/globals.css` 中定义。
   - 使用 `tailwind.config.ts` 来自定义 Tailwind CSS 配置。

### 运行

开发模式：
```
npm run dev
```

构建生产版本：
```
npm run build
```

启动生产服务器：
```
npm start
```

## 技术栈

- Next.js 14
- React 18
- TypeScript
- Tailwind CSS
- next-intl（国际化）
- next-themes（主题切换）
- Framer Motion（动画）
- React Icons

## 贡献

欢迎提交 Issues 和 Pull Requests 来改进这个项目。

## 许可证

本项目采用 MIT 许可证。详情请见 [The MIT License](https://opensource.org/license/MIT) 文件。

## 开发者信息

本项目由 [wincatcher](https://github.com/wincatcher) 开发。

如果你对这个项目感兴趣或有任何问题,欢迎通过以下方式联系我:

- GitHub: [@wincatcher](https://github.com/wincatcher)
- 电子邮件: wincatcher [at] gmail [dot] com
- 个人简介: [https://biobio.top/](https://biobio.top/)

我是一名热衷于创新和技术的独立开发者，专注于 Web 开发和人工智能应用。欢迎交流与合作!

## 支持项目

如果你觉得这个项目对你有帮助，欢迎给项目一个星标 ⭐️ 来支持它。

你也可以通过以下方式支持项目的持续开发:

- 分享项目给其他人
- 报告问题或提出改进建议
- 贡献代码或文档

感谢你的支持!

![Alt](https://repobeats.axiom.co/api/embed/08a6938436b0c5394eb7d13b0538d147f57a1876.svg "Repobeats analytics image")