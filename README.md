# mysql-
# 1.安装
## 1.更新ubuntu的软件列表
sudo apt-get uptate
PS:使用update更新软件时出现忽略、获取、命中。
hint,命中 表示链接上这个网站
get获取 表示有更新并且下载，
ign忽略 表示无更新或者更新无关紧要或者不需要

## 2.更新ubuntu的软件
sudo apt-get upgrade

## 3.安装MySQL server
sudo apt-get install mysql-server

MySQL server卸载命令：
sudo apt-get autoremove mysql-server

## 4.在安装MySQL server时让设置MySQL server 的密码

再次输入密码

## 5.安装MySQL client
sudo apt-get install mysql-client

MySQL client卸载命令：
$sudo apt autoremove mysql-client

## 6.安装libmysqlclient-dev
sudo apt-get install libmysqlclient-dev

libmysqlclient-dev卸载命令：
sudo apt autoremove libmysqlclient-dev

## 7.查看mysql是否安装成功，如果有MySQL进程则安装成功
$sudo netstat -tap |grep mysql

## 8.进入MySQL
mysql -uroot -p
