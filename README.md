# mysql-
# 1.安装
安装前，检测系统是否自带安装 MySQL:
rpm -qa | grep mysql
如果你系统有安装，那可以选择进行卸载:
rpm -e mysql　　// 普通删除模式
rpm -e --nodeps mysql　　// 强力删除模式，如果使用上面命令删除时，提示有依赖的其它文件，则用该命令可以对其进行强力删除
