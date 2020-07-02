# Update & Upgrade

Updates and upgrades are one of the maintenance tasks for system. Programs that are not upgraded for a long time, like buildings that are not maintained for a long time, will accelerate aging and gradually lose functionality until they are unavailable.

You should know the differences between the terms **Update** and **Upgrade**([Extended reading](https://support.websoft9.com/docs/faq/tech-upgrade.html#update-vs-upgrade))
- Operating system patching is **Update**, Ubuntu16.04 to Ubuntu18.04 is **Upgrade**
- MySQL5.6.25 to MySQL5.6.30 is **Update**, MySQL5.6 to MySQL5.7 is **Upgrade**

For Moodle maintenance, focus on the following two Update & Upgrade jobs

- System update(Operating System and Running Environment) 
- Moodle upgrade 

## System Update

Run an update command to complete the system update:

``` shell
#For Centos&Redhat
yum update -y

#For Ubuntu&Debian
apt update && apt upgrade -y
```
> This deployment package is pre-configured with a scheduled task for automatic updates. If you want to remove the automatic update, please delete the corresponding Cron

## Moodle Upgrade

Moodle provided multiple upgrade methods, includes: automatic upgrade, upload source code for upgrading, using CLI for upgrading

More detail please refer to Moodle official docs [Moodle Upgrading](https://docs.moodle.org/37/en/Upgrading)