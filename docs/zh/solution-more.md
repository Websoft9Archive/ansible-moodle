# 更多...

下面每一个方案，都经过实践证明行之有效，希望能够对你有帮助

## 域名绑定

绑定域名的前置条件是：已经完成域名解析（登录域名控制台，增加一个A记录指向服务器公网IP）  

完成域名解析后，从服务器安全和后续维护考量，需要完成**域名绑定**：

Moodle 域名绑定操作步骤：

1. 使用 SFTP 工具登录云服务器
2. 修改 [虚拟机主机配置文件](/zh/stack-components.html#apache)，将其中的域名相关的值
   ```text
   #### Moodle(LAMP) bind domain #### 

     <VirtualHost *:80>
     ServerName  www.mydomain.com # 修改成您的实际域名
     DocumentRoot "/data/wwwroot/moodle"
     ...
     
   #### Moodle(LNMP) bind domain #### 

     server {
      listen 80;
      server_name moodle.example.com; # 修改成您的实际域名
     ...

   ```
3. 保存配置文件，[重启服务](/zh/admin-services.html#apache)

## 向 Moodle 注册你的网站

Moodle 初始化安装完成之后，建议注册成为 Moodle 官方网站的会员，注册好处包括：升级通知，课程共享，在线安装插件等

1. 以管理员身份登录 Moodle 后台
2. 依次打开：【网站管理】>【注册】
   ![Moodle 注册](https://libs.websoft9.com/Websoft9/DocsPicture/zh/moodle/moodle-registermd-websoft9.png)
3. 注册完成后登陆，这样你的 Moodle 与官方便建立了一个连接关系

## Moodle 语言设置

1. 以管理员身份登录 Moodle 后台
2. 依次打开：【网站管理】>【语言】
   ![Moodle 语言设置](https://libs.websoft9.com/Websoft9/DocsPicture/zh/moodle/moodle-languageset-websoft9.png)
3. 根据实际情况进行语言设置
   * 语言设置：即在线切换语言
   * 定制语言：即在线编辑语言翻译内容
   * 语言包： 即上传系统默认没有内置的语言

## Moodle 客户端

1. 以管理身份登录 Moodle 后台
2. 依次打开：【网站管理】>【移动应用程序】>【移动设备设置】
   ![moodle-apps](https://libs.websoft9.com/Websoft9/DocsPicture/zh/moodle/moodle-app-1-websoft9.jpg)
3. 将【为移动设备启用网络服务】设为 **启用** 状态；
   ![moodle-apps](https://libs.websoft9.com/Websoft9/DocsPicture/zh/moodle/moodle-app-2-websoft9.jpg)
4. 保存设置；
5. 安装 [Moodle 手机客户端](https://download.moodle.org/mobile/)
6. 打开后在地址栏输入 Moodle 的访问地址，就可以开始使用移动端
   ![moodle-apps](https://libs.websoft9.com/Websoft9/DocsPicture/zh/moodle/moodle-mobile-websoft9.png)

## Moodle 插件

Moodle 是一个非常灵活的平台，大部分核心功能以插件的形式存在，系统默认安装了400多个插件。同时，官方提供了[插件市场](https://moodle.org/plugins/)供用户作用更多功能扩展。

1. [注册 Moodle 官方账号](/zh/solution-more.html#moodle-注册)，打通你的 Moodle 与官方的连接，便于在线安装插件。

2. 以管理员身份登录 Moodle 后台

3. 依次打开：【网站管理】>【插件】，会看到**安装插件**和**插件概况**两个链接
   ![moodle 插件](https://libs.websoft9.com/Websoft9/DocsPicture/zh/moodle/moodle-plugins-websoft9.png)

   * 安装插件：安装新插件入口
   * 插件概况：查看已经安装的插件列表

4. 点击【安装插件】，提供**从Moodle插件目录安装插件**和**从ZIP文件中安装插件**两种安装插件的方式
   ![moodle 安装插件](https://libs.websoft9.com/Websoft9/DocsPicture/zh/moodle/moodle-pluginsmk-websoft9.png)

   * 从Moodle插件目录安装插件：自动跳转并登录到 Moodle 的[官方插件市场](https://moodle.org/plugins/)，便可以在线安装
   * 从ZIP文件中安装插件：需提前下载插件压缩文件，再从此处**上传**安装

5. 点击【插件概况】，列出默认安装的插件，可以进行停用、卸载等操作
   ![moodle 插件概况](https://libs.websoft9.com/Websoft9/DocsPicture/zh/moodle/moodle-plugininfo-websoft9.png)
   
6. 点击[插件概况](https://moodle.org/plugins/)寻找所需的插件，然后安装它们

> 更多插件管理查看官方文档 [Moodle Plugins](https://docs.moodle.org/37/en/Installing_plugins)

## Moodle 主题

Moodle 主题实际上是一个插件，因此需要安装新主题，必须通过【安装插件】的方式先进行安装。  

1. 以管理员身份登录 Moodle
2. 依次打开：【网站管理】>【插件】，进入插件市场后，选择【Theme】类型的插件
   ![](https://libs.websoft9.com/Websoft9/DocsPicture/zh/moodle/moodle-mktheme-websoft9.png)

3. 在线安装所需的主题

3. 打开【网站管理】>【外观】>【主题选择器】
   ![](https://libs.websoft9.com/Websoft9/DocsPicture/zh/moodle/moodle-addtheme001-websoft9.png)

4. 点击【更改主题】即可完成主题更换
   ![](https://libs.websoft9.com/Websoft9/DocsPicture/zh/moodle/moodle-addtheme002-websoft9.png)

## 重置密码

常用的 Moodle 重置密码相关的操作主要有修改密码和找回密码两种类型：

### 修改密码

1. 登录 Moodle 后台，点击头像，进入【个人档案】设置下的**小齿轮图标**
  ![Moodle 修改密码](https://libs.websoft9.com/Websoft9/DocsPicture/zh/moodle/moodle-modifypw-websoft9.png)

2. 点击【更改密码】链接，开始修改密码

### 找回密码

如果用户忘记了密码，有两种找回密码的方案：

* 登录界面通过邮件找回密码（需提前完成 [SMTP 设置](/zh/solution-smtp.md)）
* 数据库中重置密码两种方案

下面介绍通过数据库找回密码的方案：

1. 登录 [phpMyAdmin](/zh/admin-mysql.md)，并找到你的网站数据库下的 *mdl_user*表

  ![Moodle user表](https://libs.websoft9.com/Websoft9/DocsPicture/zh/moodle/moodle-phpmyadminuser-websoft9.png)

2. 编辑【admin】用户，将其中的 `password` 字段的值用 `21232f297a57a5a743894a0e4a801fc3` 替换

3. 点击【执行】，新的密码就被重置为`admin`
