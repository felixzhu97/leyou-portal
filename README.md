# Leyou Portal

乐优商城前端门户系统

## 项目简介

乐优商城是一个 B2C 电商平台的前端门户系统，包含商品展示、购物车、订单管理等功能模块。

## 安装与运行

1. 克隆项目：

```bash
git clone https://github.com/zhuzhiqiang997/leyou-portal.git
```

2. 安装依赖：

```bash
npm install
```

3. 启动开发服务器：

```bash
npm start
```

服务器将在 http://localhost:10002 启动

## 项目结构

```
leyou-portal/
├── css/                  # 样式文件
├── fonts/                # 字体图标
├── img/                  # 图片资源
├── js/                   # JavaScript脚本
├── plugins/              # 第三方插件
├── items/                # 商品数据
├── index.html            # 首页
├── item.html             # 商品详情页
├── cart.html             # 购物车页
├── search.html           # 搜索页
├── login.html            # 登录页
├── register.html         # 注册页
└── package.json          # 项目配置
```

## 主要功能页面

- 首页 (index.html)
- 商品详情 (item.html)
- 购物车 (cart.html)
- 搜索 (search.html)
- 登录/注册 (login.html, register.html)
- 订单管理 (home-order\*.html)
- 个人中心 (home-person\*.html)

## 技术栈

- HTML5
- CSS3
- JavaScript
- Vue.js (部分页面)
- Axios (HTTP 请求)
- Live Server (开发服务器)

## 贡献指南

1. Fork 本仓库
2. 创建特性分支 (`git checkout -b feature/你的特性`)
3. 提交修改 (`git commit -am '添加新特性'`)
4. 推送分支 (`git push origin feature/你的特性`)
5. 创建 Pull Request
6. 
## 开源协议

[MIT](https://opensource.org/licenses/MIT)