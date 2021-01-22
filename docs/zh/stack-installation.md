# 初始化安装

在云服务器上部署 Moodle 预装包之后，请参考下面的步骤快速入门。

## 准备

1. 在云控制台获取您的 **服务器公网IP地址** 
2. 在云控制台安全组中，检查 **Inbound（入）规则** 下的 **TCP:80** 端口是否开启
3. 若想用域名访问 Moodle，请先到 **域名控制台** 完成一个域名解析

## Moodle 安装向导

1. 使用本地电脑的 Chrome 或 Firefox 浏览器访问网址：*http://域名* 或 *http://Internet IP*, 就进入引导首页
2. 根据系统提示，选择语言，进入下一步 
   ![](https://libs.websoft9.com/Websoft9/DocsPicture/zh/moodle/moodle-install001-websoft9.png)

3. 选择数据库类型，默认为【改进的MySQL】，然后进入确认路径设置（保持默认设置），进入下一步 
   ![](https://libs.websoft9.com/Websoft9/DocsPicture/zh/moodle/moodle-install002-websoft9.png)

4. 填写数据库连接信息，建议采用预装环境自带的 MySQL 数据库([不知道账号密码？](/zh/stack-accounts.html#mysql))
   ![](https://libs.websoft9.com/Websoft9/DocsPicture/zh/moodle/moodle-install003-websoft9.png)

5. 经过几次确认后，安装进入环境检测步骤，继续后续步骤 
   ![](https://libs.websoft9.com/Websoft9/DocsPicture/zh/moodle/moodle-install004-websoft9.png)

6. 设置后台账号信息，请务必设置好并牢记之。进入下一步 
   ![](https://libs.websoft9.com/Websoft9/DocsPicture/zh/moodle/moodle-install005-websoft9.png)

7. 设置网站初始化信息 
    ![](https://libs.websoft9.com/Websoft9/DocsPicture/zh/moodle/moodle-install006-websoft9.png)

8. 跟随安装提示直到完成，过程中尽量选择默认设置，勾选安装所有模块

9. 系统完成最后一步安装，建议进入 Moodle 后台（以管理身份登录即进入后台），体验完整功能 
   ![](https://libs.websoft9.com/Websoft9/DocsPicture/zh/moodle/moodle-install007-websoft9.png)

10. [注册 Moodle 官方账号](/zh/solution-more.html#moodle-注册)，打通你的 Moodle 与官方的连接，便于在线安装插件。

> 需要了解更多Moodle的使用，请参考官方文档：[Moodle Documentation](https://docs.moodle.org)

## Moodle 入门向导

下面通过一个创建一个课程范例，来快速介绍 Moodle 的使用：

## 常见问题

#### 浏览器打开IP地址，无法访问 Moodle（白屏没有结果）？

您的服务器对应的安全组80端口没有开启（入规则），导致浏览器无法访问到服务器的任何内容

#### 本部署包采用的哪个数据库来存储 Moodle 数据？

是MySQL

#### 是否可以采用云厂商提供的 RDS 来存储 Moodle 数据？

可以
