# ITResHub

ITResHub 是一个专注于 IT 资源分享的社区平台，致力于为开发者、运维人员和 IT 爱好者提供便捷的资源发现与分享环境。

在这里，你可以找到最新的云服务器优惠、大模型 API 折扣、实用开发工具和技术教程，也可以发布自己发现的优质资源，与社区共同成长。

## 核心功能

- 资源发现：按分类、厂商、关键词筛选资源并支持排序与分页
- 资源互动：点赞、收藏、评论、举报与分享
- 资源发布：用户可提交资源，支持新增自定义厂商并进入审核流程
- 文档中心：支持分类与语言筛选，提供内容浏览体验
- 管理后台：资源审核、举报处理、角色管理与统计看板
- Agent 能力：提供面向 AI Agent 的资源与文档 API

## 技术栈

- 前端：React 18 + TypeScript + Vite + Tailwind CSS + Zustand
- 后端：Express + TypeScript（tsx/nodemon）
- 数据层：Supabase
- 其他：i18next、React Router、Recharts

## 快速开始

### 1) 安装依赖

```bash
npm install
```

### 2) 配置环境变量

在项目根目录创建 `.env`，至少配置以下变量：

```bash
VITE_SUPABASE_URL=
VITE_SUPABASE_ANON_KEY=
VITE_API_URL=
SUPABASE_URL=
SUPABASE_SERVICE_ROLE_KEY=
PORT=3001
```

### 3) 启动开发环境

```bash
npm run dev
```

该命令会并行启动：

- 前端开发服务（Vite）
- 后端开发服务（Express）

## 可用脚本

```bash
npm run dev          # 前后端并行开发
npm run client:dev   # 仅启动前端
npm run server:dev   # 仅启动后端
npm run build        # 构建前端产物
npm run preview      # 预览构建产物
npm run check        # TypeScript 类型检查
npm run lint         # ESLint 检查
npm run edge:start   # 启动边缘代理脚本
```

## 项目结构

```text
.
├─ src/                # 前端源码（页面、组件、状态、国际化等）
├─ api/                # 后端源码（路由、控制器、服务）
├─ public/             # 静态资源与插件清单
├─ supabase/           # 数据库迁移与相关配置
├─ scripts/            # 辅助脚本
└─ dist/               # 前端构建产物
```


## 贡献指南

欢迎提交 Issue 与 Pull Request 来帮助改进 ITResHub。建议在提交前执行：

```bash
npm run check
npm run lint
npm run build
```

## License

当前仓库未设置开源许可证，如需开源建议补充 `MIT` 或其他许可证。
