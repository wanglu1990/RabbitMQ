### Windows下安装php扩展ampq



##### 安装前准备工作：

1.  查看本地PHP版本

    ![avatar](https://raw.githubusercontent.com/wanglu1990/RabbitMQ/master/images/phpinfo.png)

2.  下载对应版本的ampq
    
    地址：<http://pecl.php.net/package/amqp>
    
    
    ![avatar](https://raw.githubusercontent.com/wanglu1990/RabbitMQ/master/images/select_amqp_extension.png)

##### 安装方法如下：


1.  复制php_amqp.dll到php/ext，如C:\xampp\php\ext目录下

2.  php.ini中添加extension=php_amqp.dll

3.  复制rabbitmq.1.dll到php目录 如C:\xampp\php目录下

4.  修改apache配置文件httpd.conf，添加LoadFile  "C:/xampp/php/rabbitmq.1.dll"

5.  重启apache，phpinfo()查看下是否支持amqp扩展

    ![avatar](https://raw.githubusercontent.com/wanglu1990/RabbitMQ/master/images/amqp_extension.png)

