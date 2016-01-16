# jfinal cms
------------------------

#### 网站地址：[http://www.jflyfox.com/mtg](http://www.jflyfox.com/mtg) ####
#### 管理地址：http://yourip/admin  ####
#### 测试账号: admin/admin123 或 test/123456  ####

# 一、平台部署说明 #
------------------------
> 1. 数据库配置文件：src/conf/db.properties
> 2. 安装mysql数据库，创建用户和数据库。
> 3. 运行mysql.sql文件。
> 4. 如需要oauth2的，设置src/conf/oauth.properties

# 鸣谢
 1. [JFinal](http://www.oschina.net/p/jfinal)
 2. [beetl](http://ibeetl.com/community/)
 3. [oschina](http://www.oschina.net/)

# 更新说明
>## 2016-01-16
> 1. 升级为2.3.0。
> 2. 项目全面重构，jfinal升级为2.1。
> 3. 后台管理支持列表排序查询功能。
> 4. 加入项目基类model和controller解决和依赖包基类重复代码覆盖问题。

>## 2016-01-15
> 1. 名字更新，升级为2.2.0

>## 2016-01-14 mtgxxw2.1.1
> 1. 升级父类依赖，升级为2.1.1

>## 2016-01-03 mtgxxw2.1.0
> 1. 代码全面重构，优化目录结构，升级为2.1
> 2. 加入日志管理，记录后台增删改查以及登陆登出操作。
> 3. 完善前台目录url美化。

>## 2015-12-27
> 1. 修复评论分页显示bug

>## 2015-11-29 mtgxxw2.0.0
> 1. 主要讲jfinal升级为2.0

>## 2015-09-26
> 1. 加入文章附件功能：确保存在download目录（tmp临时目录，image_url图片目录，file_url附件目录）
> 在文章修改目录进行上传和删除操作，附件只支持一个文件，现在是可以上传所有类型。

>## 2015-09-21
> 1. 实现文章缓存自动更新，解决文章发布不可以见问题（需要后台点击更新缓存）。
> config.properties文件中可以配置MTG.UPDATE_TIME字段更新时间，单位毫秒；配置0为不更新。
> 2. 修复用户发布文章中更新时间为空问题。

>## 2015-08-16 mtgxxw1.4.2
> 1. 加入喜欢的文章。
> 2. 解决cookie访问异常，导致页面无法访问问题。
> 3. 修改我的空间页面布局。

>## 2015-08-04
> 1. 感谢老李提醒，mysql5.1中group_concat可能到返回类型是blob而不能转换为String，mysql5.5没有这个问题。
可以通过CAST(group_concat(tagname) AS CHAR)进行优化，未进行测试。

>## 2015-08-03
> 1. 修复cookie获取权限后，导致后台菜单加载失败问题。

>## 2015-08-02 mtgxxw1.4.1
> 1. 加入用户cookie，避免重启服务用户信息失效以及关闭浏览器失效问题
> 2. 修改登陆页面与页面风格保持一致，加入验证码。
> 3. 修复我的空间页面bug。
> 4. 修复首页跳转bug。

>## 2015-06-21 mtgxxw1.4
> 1. 用户登陆后可以进行博文发布、编辑、删除，发布加入字符限制。
> 2. Ueditor图片上传加入大小和数量限制。
> 3. 加入非法上传用户记录。

>## 2015-06-13 mtgxxw1.3
> 1. 优化首页，加入最新新闻和最新动态切换。
> 2. 优化头像点击展示。

>## 2015-06-09 mtgxxw1.2
> 1. 发布1.2版本，主要是bug修复。
> 2. 感谢fxhover同学，修复漏洞：http://www.jflyfox.com/mtg/front/tags/%3Cimg%20%20src=%22xx%22%20onerror=%22alert%28111%29;%22%3E111

>## 2015-06-06
> 1. 加入点击用户查看信息。

>## 2015-06-04
> 1. jflyfox_jfinal升级为2.1,全面去除模板，更简单易懂
> 2. 登录名称错误修改。
> 3. 优化文章编辑操作。

>## 2015-06-03 mtgxxw1.1
> 1. 发布1.1版本，这次主要优化前台访问速度。
> 2. 加入cdn，如果本地没有网络请修改/static/component/include/jquery.html和/static/component/include/bootstrap.html。

>## 2015-06-02
> 1. 回复管理加入排序。
> 2. 前台查看加入伪静态化。
> 3. 优化用户部门，加入第三方注册部门。
> 4. 根据加载慢问题，加入外链图片加载，缓解前台带宽问题。首页加入网络图片，后台加入编辑。

>## 2015-05-31 mtgxxw1.0
> 1. 基本功能页面已完成，可以进行开源。
> 2. 如还包含私人数据，希望大家提醒我进行删除。

>## 2015-05-27
> 1. 完善首页和菜单seo。
> 2. 优化model，加入get set方法。
> 3. 加入评论数和浏览量计数缓存。
> 4. 完善关于我们。
> 5. 功能已基本完善，待完善数据。


>## 2015-05-26
> 1. 已完成初稿，基本可以使用。
> 2. 加入菜单url优化，简洁美观。
> 3. 加入伪静态化，看着更高大上。

>## 2015-05-25
> 1. 初始化，完成首页


# 开源赞助
![OSC@GIT](http://static.oschina.net/uploads/space/2015/0213/104940_ZKNb_166354.png "开源赞助我(支付宝)")
