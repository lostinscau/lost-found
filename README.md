# 失物招领

---

这是一个使用nodejs在微信公众平台上开发的一个网页型应用。任何关注了微信公众号的人都可以在上面发布失物信息，包括

- 标题
- 失物描述
- 联系方式
- 微信昵称
- 微信头像

---

### 使用方法

- 安装nodejs环境和mongodb数据库
- git clone本项目
- 进入lost-found文件夹，使用npm install命令安装依赖包
- 修改index.js文件
  - 替换`var client = new OAuth('appid', 'appsecret')`里面的appid和appsecret
  - 在mongodb里面建立数据库，并把`mongodb://localhost:27017/test`里面的`test`替换为新建的数据库的名字
  - 替换`var url = client.getAuthorizeURL('site', 'STATE', 'snsapi_userinfo')`里面的`site`为自己的域名
- 在微信公众号里添加菜单指向该应用

---

### 应用截图

![home](https://raw.githubusercontent.com/lostinscau/lost-found/master/screenshots/home.png)
![add](https://raw.githubusercontent.com/lostinscau/lost-found/master/screenshots/add.png)
![show](https://raw.githubusercontent.com/lostinscau/lost-found/master/screenshots/show.png)
