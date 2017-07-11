###rebbitmq安装


安装过程如下：

1. 下载文件，地址<https://www.rabbitmq.com/install-windows.html>

2. 安装后文件路径

    ![avatar](https://raw.githubusercontent.com/wanglu1990/RabbitMQ/master/images/rebbitmq_server.png)


3. 启动监控管理插件服务

```
rabbitmq-plugins enable rabbitmq_management

```

![avatar](https://raw.githubusercontent.com/wanglu1990/RabbitMQ/master/images/manage_plugins.png)


 看到6个plugins已经安装接下来。

4. 访问http://localhost:15672/#/（用户名：guest 密码：guest)查看rebbitmq信息

  ![avatar](https://raw.githubusercontent.com/wanglu1990/RabbitMQ/master/images/login_rebbitmq.png)
      
      
  ![avatar](https://raw.githubusercontent.com/wanglu1990/RabbitMQ/master/images/look_rebbitmq_info.png)


5. 运行服务

```
rabbitmq-server.bat start

```

6. 停止服务
```
rabbitmqctl.bat stop

```

7. 查看用户

```
rabbitmqctl.bat list_users

```

![avatar](https://raw.githubusercontent.com/wanglu1990/RabbitMQ/master/images/list_users.png)


