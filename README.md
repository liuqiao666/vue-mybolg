# vue-mybolg
vue2.0+vue-router+mongoDB+koa2+vuex+响应式布局=前后端分离的个人博客

## 主要技术构成
前端主要技术栈为vue.js、vue-router、 vue-resource、 vuex

后端主要技术栈为node.js、 mongodb

## 博客功能
### 前台页面
- 搜索文章
- 动态显示文章
- 留言
- 文章分类显示
- 评论文章
- 文章目录

### 后台管理页面
- 发布文章
- 存为草稿
- 搜索文章
- 修改账户
- 权限验证
- 登录验证
- markdown编辑器

运行环境
- node.js
- mongoDB


克隆远程库
```
git clone https://github.com/liuqiao666/vue-mybolg

进入项目目录vue-mybolg后，安装依赖
```
npm install

安装项目前请先安装数据库，然后启动mongodb。（不要关闭当前窗口，然后重新打开另外一个dos窗口，进行下一个步骤）
```
mongod --dbpath E:\mongodb\data     // E:\mongodb\data 为数据库文件夹位置，可自行设置
```
运行服务器。（确保数据库mongodb已经启动，不要关闭当前窗口，然后回到之前的dos窗口，进行下一个步骤）
```
npm run start
```
在8082端口热重载开发，等待一会后，会自动弹出浏览器窗口，加载会比较慢，请耐心等待
```
npm run dev

### 注意
- 账户： liuqiao    密码： 666
- 配置： 请将server/app.js和/server/api/comment.js里面的xxx@qq.com改为自己的邮箱，来测试邮箱通知功能
- 邮箱通知功能，我注册了一个公用126邮箱去发送邮件，如果频繁发送邮件到一固定邮箱，则会被当成垃圾邮件被系统拦截。
- 登录界面在：最底下的——‘站长登录’
