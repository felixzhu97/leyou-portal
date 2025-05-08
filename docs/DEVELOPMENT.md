# 开发指南

## 环境要求

- Node.js 14+
- npm 6+
- Git

## 开发流程

1. 克隆仓库

```bash
git clone https://github.com/zhuzhiqiang997/leyou-portal.git
```

2. 安装依赖

```bash
npm install
```

3. 启动开发服务器

```bash
npm start
```

4. 开发新功能时请创建新分支

```bash
git checkout -b feature/your-feature-name
```

5. 提交代码前运行测试

```bash
npm test
```

## 代码规范

- 遵循 ESLint 规则
- 组件使用 PascalCase 命名
- 方法使用 camelCase 命名
- 提交信息遵循 Conventional Commits 规范

## 调试技巧

- 使用 Chrome DevTools 调试前端代码
- 查看控制台日志定位问题
- 使用 Vue DevTools 调试 Vue 组件
