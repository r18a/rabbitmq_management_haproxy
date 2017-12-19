## Basic haproxy configuration for rabbitmq_management

|         | Version           |
| ------------- |:-------------:|
| haproxy      | 1.5.18 |
| rabbitmq      | 3.6.6      |

Forward to TCP Port 15672 (RabbitMQ Management Console)
```
semanage port -m -t http_port_t -p tcp 15672
```
and/or
```
firewall-cmd --zone=public --add-port=15672/tcp --permanent
```
