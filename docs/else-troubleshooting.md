# Troubleshooting

If you're having trouble with running RabbitMQ, here is a quick guide to solve most common problems.

> Most faults about the Instance is closely related to the Instance provider, Cloud Platform. Provided you're sure the fault is caused by Cloud Platform, refer to [Cloud Platform Documentation](https://support.websoft9.com/docs/faq/tech-instance.html).

#### How can I check the error logs?

You can find the keywords **Failed** or **error** from the logs directory: `/data/logs`

#### Moodle can't start?

Insufficient disk space and memory, incorrect configuration file may cause the failure to start the service. 

It is recommended to first check through the command.

```shell
# service status
systemctl status mysql
systemctl status apache

# view disk space
df -lh

# view memory rate
free -lh
```

#### Repair a corrupted Moodle database

The problem can be repaired using the mysqlcheck command

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