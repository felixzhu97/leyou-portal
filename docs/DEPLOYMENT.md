# 部署指南

## 生产环境要求

- Node.js 14+
- Nginx 1.18+
- Linux 服务器
- 至少 2GB 内存

## 构建步骤

1. 安装依赖

```bash
npm install --production
```

2. 构建静态资源

```bash
npm run build
```

3. 构建产物将生成在`dist`目录

## Nginx 配置

```nginx
server {
    listen 80;
    server_name your-domain.com;

    location / {
        root /path/to/dist;
        index index.html;
        try_files $uri $uri/ /index.html;
    }
}
```

## 环境变量

创建`.env.production`文件配置生产环境变量：

```
VUE_APP_API_URL=https://api.your-domain.com
VUE_APP_BASE_URL=/
```

## 部署流程

1. 将构建产物上传到服务器
2. 配置 Nginx
3. 启动 Nginx 服务
4. 配置 HTTPS 证书(推荐使用 Let's Encrypt)
