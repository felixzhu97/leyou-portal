# API 文档

## 基础信息

- 基础 URL: `https://api.your-domain.com`
- 认证方式: JWT
- 默认响应格式: JSON

## 用户认证

### 登录

- 路径: `/auth/login`
- 方法: POST
- 请求示例:

```json
{
  "username": "user@example.com",
  "password": "yourpassword"
}
```

- 响应示例:

```json
{
  "token": "eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9...",
  "expiresIn": 3600
}
```

## 商品接口

### 获取商品列表

- 路径: `/api/items`
- 方法: GET
- 参数:
  - page: 页码
  - size: 每页数量
- 响应示例:

```json
{
  "total": 100,
  "items": [
    {
      "id": 1,
      "name": "商品名称",
      "price": 99.9,
      "image": "/images/item1.jpg"
    }
  ]
}
```

## 错误码

| 状态码 | 说明           |
| ------ | -------------- |
| 400    | 请求参数错误   |
| 401    | 未授权         |
| 404    | 资源不存在     |
| 500    | 服务器内部错误 |
