# Configuration RSYSLOG

```
$ cat /etc/rsyslog.d/syslog.conf
*.* @<host ELK>:<port Logstash>
```shell

