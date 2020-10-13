# MySql8.21
参考博客：https://blog.csdn.net/wangbeibei23/article/details/82056951
MySql官网下载地址：https://dev.mysql.com/downloads/mysql/
第一步：
	1、下载之后直接解压 到安装目录即可 ；
	2、配置环境变量(D:\Program Files\Mysql\mysql-8.0.21-winx64\bin) ;
第二步：
	初始化数据库(mysqld --initialize --console)
	命令执行后会在和bin同级目录下产生data文件，即是root账号对应的数据库并产生随机密码(没记住初始密码可以删掉初始化的 data目录，再执行一遍初始化命令又会重新生成的)
服务名：mysql
密码：password
第三步：
	在bin目录下执行安装服务命令(mysqld --install [服务名])，服务名可以不写默认的名字为 mysql。
第四步：启动服务(net start mysql)
第五步：登录数据库(mysql -u root -p)
第六步：更改密码(ALTER USER 'root'@'localhost' IDENTIFIED WITH mysql_native_password BY '新密码';)

常见问题：
	1、发生系统错误 2，系统找不到指定的文件(https://blog.csdn.net/will__be/article/details/107540487)
	2、发生系统错误 5，拒绝访问(https://www.cnblogs.com/zhangqingwang/p/10667110.html)
	3、找不到vcruntime140_1.dll,无法继续执行代码(https://blog.csdn.net/littlehaes/article/details/104127787)【补丁文件】
