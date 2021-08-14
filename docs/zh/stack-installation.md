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

Moodle 是以课程为中心的组织模式，围绕课程的创建、关联老师和学生，开展教学和学习活动，来构建强大的在线学习管理平台。Moodle 通过对课程关联资源和活动，来设置课程的PPT、视频等教学资源和作业、考试、反馈等教学活动。Moodle 还有提供很多实用的功能，如更多的系统选项、课程能力模型、成绩报告及更多的课程活动等。

**角色**：Moodle 系统的主要角色有3类，分别是管理员admin，老师，学生。

管理员拥有最高权限，是系统管理员和学校校长，负责系统、成员、课程、权限分配等管理。

**课程**：课程是 Moodle 的核心要素，也可以理解为班级。

- 通过课程关联学生和老师，老师开展教学管理，学生开展学习、考试、讨论等学习活动；

- 通过课程关联资源和活动，资源如教学PPT、音像、题库等，活动如作业、测试、反馈、评价等教学活动；

1、系统管理：登录进入系统，选择【网站管理】进行系统管理、用户管理及课程管理等。
   ![img](https://libs.websoft9.com/Websoft9/blog/tmp/moodle/zh/moodle-system-manage-websoft9.png)

2、用户管理：进入【网站管理】后，通过【用户】选项，添加用户
   ![img](https://libs.websoft9.com/Websoft9/blog/tmp/moodle/zh/moodle-user-manage-websoft9.png)
   
3、添加课程：进入【网站管理】后，通过【课程】选项，添加新课程
   ![img](https://libs.websoft9.com/Websoft9/blog/tmp/moodle/zh/moodle-course-manage-websoft9.png)

4、课程管理：通过【站点首页】 点击【可用的课程】 java 进入课程管理
   ![img](https://libs.websoft9.com/Websoft9/blog/tmp/moodle/zh/moodle-course-manage1-websoft9.png)
   
   在课程管理主页，通过【设置】【更多】进行课程管理
   ![img](https://libs.websoft9.com/Websoft9/blog/tmp/moodle/zh/moodle-course-manage2-websoft9.png)
   ![img](https://libs.websoft9.com/Websoft9/blog/tmp/moodle/zh/moodle-course-manage3-websoft9.png)
   
5、课程关联老师和学生：通过【参与人】设置，关联老师和学生。点击【参与人】进入人员管理，通过【加入用户】选择用户参与课程，编辑【角色】设置用户角色
   ![img](https://libs.websoft9.com/Websoft9/blog/tmp/moodle/zh/moodle-course-teacher-student-websoft9.png)
   
6、课程关联资源和活动：点击课程名称，进入课程主页，点击【打开编辑功能】，关联课程资源和活动
   ![img](https://libs.websoft9.com/Websoft9/blog/tmp/moodle/zh/moodle-course-resource-websoft9.png)
   
   通过设置课程的章节、主题，然后点击章节右下方的【添加一个活动或资源】，可以是文件资源也可以是考试等教学活动
   ![img](https://libs.websoft9.com/Websoft9/blog/tmp/moodle/zh/moodle-course-resource1-websoft9.png)
   ![img](https://libs.websoft9.com/Websoft9/blog/tmp/moodle/zh/moodle-course-resource2-websoft9.png)
   
7、题库管理：测试与题库管理：Moodle 可以方便的添加测试，测试可以从题库中随机选题，也可以现场组卷。通过【更多】进入课程主页，选择下方题库进行题库管理
   ![img](https://libs.websoft9.com/Websoft9/blog/tmp/moodle/zh/moodle-course-question-websoft9.png)
   ![img](https://libs.websoft9.com/Websoft9/blog/tmp/moodle/zh/moodle-course-question1-websoft9.png)
   
   新建题目，把正确的选项的得分设为100%就是设置正确答案
   ![img](https://libs.websoft9.com/Websoft9/blog/tmp/moodle/zh/moodle-course-question2-websoft9.png)
   ![img](https://libs.websoft9.com/Websoft9/blog/tmp/moodle/zh/moodle-course-question3-websoft9.png)
   
8、测试管理：测试管理是针对某个章节，添加【测试】活动，组织题目，开展课程测试
   ![img](https://libs.websoft9.com/Websoft9/blog/tmp/moodle/zh/moodle-course-test-websoft9.png)
   
   添加测试，命名保存
   ![img](https://libs.websoft9.com/Websoft9/blog/tmp/moodle/zh/moodle-course-test1-websoft9.png)
   
   编辑测试，通过“添加”设置试题及细节
   ![img](https://libs.websoft9.com/Websoft9/blog/tmp/moodle/zh/moodle-course-test2-websoft9.png)
   ![img](https://libs.websoft9.com/Websoft9/blog/tmp/moodle/zh/moodle-course-test3-websoft9.png)
   
   设置完后，在对应的“基础语法”章节中有了“Test3”的教学测试活动，学生可以参与考试了
   ![img](https://libs.websoft9.com/Websoft9/blog/tmp/moodle/zh/moodle-course-test4-websoft9.png)
   

## 常见问题

#### 浏览器打开IP地址，无法访问 Moodle（白屏没有结果）？

您的服务器对应的安全组80端口没有开启（入规则），导致浏览器无法访问到服务器的任何内容

#### 本部署包采用的哪个数据库来存储 Moodle 数据？

是MySQL

#### 是否可以采用云厂商提供的 RDS 来存储 Moodle 数据？

可以
