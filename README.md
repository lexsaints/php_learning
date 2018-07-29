# php_learning
php学习记录
.configure --prefix=/usr/local/php/ #配置安装路
Linux Windows系统下相关安装记录及配置方法
php.ini文件打开cgi.fix_pathinfo=0;修改该行
注意:①/usr/local/php/etc/php-fpm.conf配置文件 可以修改为自定义的用户和组，但是也可以使用默认的nobody，不影响。
     ②/usr/local/etc/php-fpm.conf修改最后一行，最后一行引用了安装路径下/usr/local/php/etc/php-fpm.d/*.conf所有文件，但是初始安装之后，该路径下并没有.conf结尾的文件，只有www.conf.default;将 mv www.conf.default www.conf,如果不修改 启动./php-fpm时 将会报错php-fpm.d下找不到conf文件，无法启动。
