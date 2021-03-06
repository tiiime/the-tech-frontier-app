# 开发技术前线 Android 客户端需求文档

## 功能需求

1. 用户进入App，首先获取前50篇文章记录，显示文章标题、作者、阅读量、创建时间；
2. 下拉到最底部时加载后50条数据；
3. 用户点击某篇文章后跳转到文章阅读页面，通过webview加载相关内容；
4. 文章内容缓存到本地数据库;
5. 用户在主页可以通过左右滑动切换tab，含有Android、iOS、招聘信息、加入我们四个tab；
6. 用户可以通过第三方社交平台登录，可以分享文章到社交平台(微博、QQ、QQ空间、朋友圈、微信)；
7. 用户可以收藏文章，需要在菜单项中增加一个收藏菜单，用以切换到收藏的文章列表。

## 数据库设计

1. 文章缓存表-articles,存储文章的实体信息；
2. 文章收藏表-favorates,与articles不同的是这里需要一个用户id来标识文章属于哪个用户,这个用户id可以通过第三方平台获取到，例如openid;
3. 用户表，存储用户信息，包括用户id、用户名、token等。


## 界面版式图

| ![](document/images/material.png) | ![](document/images/material-menu.png) |
|--------|--------|
| 主界面 | 菜单界面 |