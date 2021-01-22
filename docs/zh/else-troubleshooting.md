# 故障处理

此处收集使用 Moodle 过程中最常见的故障，供您参考

> 大部分故障与云平台密切相关，如果你可以确认故障的原因是云平台造成的，请参考[云平台文档](https://support.websoft9.com/docs/faq/zh/tech-instance.html)

#### 如何查看错误日志？

日志文件路径为：`/data/logs`。检索关键词 **Failed** 或者 **error** 查看错误

#### 数据库服务无法启动

数据库服务无法启动最常见的问题包括：磁盘空间不足，内存不足，配置文件错误。  
建议先通过命令进行排查  

```shell
# 查看磁盘空间
df -lh

# 查看内存使用
free -lh

# 查看服务状态和日志
systemctl status mysql
```

#### 修复数据库错误

出现数据库需要修复的提示，请参考下面的命令修复对应的数据库表  

```
#mysqlcheck -u moodleuser -p --auto-repair moodle
Enter password:
moodle.adodb_logsql                      OK
moodle.mdl_assignment                    OK
moodle.mdl_assignment_submissions        OK
...
moodle.mdl_log
error    : Table './moodle/mdl_log' is marked as crashed and should be repaired
...
moodle.mdl_sessions2
error    : Table './moodle/mdl_sessions2' is marked as crashed and should be repaired

Repairing tables
moodle_18_latest.mdl_log                           OK
moodle_18_latest.mdl_sessions2                     OK
```