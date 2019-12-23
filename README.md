# README

## 项目启动

```bash
# install dependencies
yarn install

# Start MongoDB (windows)
mongod

# run server at http://localhost:3000

yarn dev
```

## 功能设计

1. 注册
   1. 注册页：`GET /signup`
   2. 注册（包含上传头像）：`POST /signup`
2. 登录
   1. 登录页：`GET /signin`
   2. 登录：`POST /signin`
3. 登出：`GET /signout`
4. 查看文章
   1. 主页：`GET /posts`
   2. 个人主页：`GET /posts?author=xxx`
   3. 查看一篇文章（包含留言）：`GET /posts/:postId`
5. 发表文章
   1. 发表文章页：`GET /posts/create`
   2. 发表文章：`POST /posts/create`
6. 修改文章
   1. 修改文章页：`GET /posts/:postId/edit`
   2. 修改文章：`POST /posts/:postId/edit`
7. 删除文章：`GET /posts/:postId/remove`
8. 留言
   1. 创建留言：`POST /comments`
   2. 删除留言：`GET /comments/:commentId/remove`

### 参考链接

- https://github.com/nswbmw/N-blog
- https://github.com/fengshi123/express_project
- https://github.com/i5ting/mvc
