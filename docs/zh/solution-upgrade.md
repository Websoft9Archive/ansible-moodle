# 更新升级

网站技术日新月异，**更新升级**是维护工作之一，长时间不升级的程序，就如长时间不维护的建筑物一样，会加速老化、功能逐渐缺失直至无法使用。  

这里注意更新与升级这两词的差异（[延伸阅读](https://support.websoft9.com/docs/faq/zh/tech-upgrade.html#更新-vs-升级)），例如：
- 操作系统打个补丁常称之为**更新**，Ubuntu16.04 变更为 Ubuntu18.04，称之为**升级**
- MySQL5.6.25-->MySQL5.6.30 常称之为**更新**，MySQL5.6->MySQL5.7 称之为**升级**

Moodle 完整的更新升级包括：系统级更新（操作系统和运行环境）和 Moodle 程序升级两种类型

## 系统级更新

运行一条更新命令，即可完成系统级更新：

``` shell
#For Centos&Redhat
yum update -y

#For Ubuntu&Debian
apt update && apt upgrade -y
```
> 本部署包已预配置一个用于自动更新的计划任务。如果希望去掉自动更新，请删除对应的Cron


## Moodle升级

Moodle 官方提供了多种升级方式（[Moodle Upgrading](https://docs.moodle.org/37/en/Upgrading)），包括上传代码升级和命令升级等方式。  

下面我们以命令行升级方式为例，介绍升级的大致方案：

1. 提前做好代码和数据库备份

2. 使用 SSH 远程登录到 Moodle 服务器，运行如下的命令开始升级：
   ```
   cd /data/wwwroot/moodle/admin/cli
   php upgrade.php
   ```
3. 等待升级完成