# mysql-
# 1.安装

## 1.安装MySQL server
sudo apt-get install mysql-server
MySQL server卸载命令：
sudo apt-get autoremove mysql-server

## 2.安装MySQL client
sudo apt-get install mysql-client
MySQL client卸载命令：
$sudo apt autoremove mysql-client

## 3.安装libmysqlclient-dev
sudo apt-get install libmysqlclient-dev
libmysqlclient-dev卸载命令：
sudo apt autoremove libmysqlclient-dev

## 4.查看mysql是否安装成功，如果有MySQL进程则安装成功
$sudo netstat -tap |grep mysql

## 5.进入MySQL
mysql -u root -p

# ps:关于安装过程没有输入密码的情况，用以下命令解决，里面记录了用户名和密码
sudo vim /etc/mysql/debian.cnf

## 关于修改用户名和密码
update mysql.user set authentication_string=password('password') where user='root'and Host = 'localhost';

# PS：重启/打开/关闭MySQL的方法是：sudo service mysql restart/start/stop

# 关于卸载mysql，如果没有卸载完全，则可尝试如下命令（没有验证）
dpkg -l |grep ^rc|awk '{print $2}' |sudo xargs dpkg -P
