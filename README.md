# Configuration-on-server

1.创建用户

adduser newname

2.设置密码

passwd newname

3.修改用户所属组

usermod -G groups newname

4.修改文件所属者和权限

chown -R newname:groups filename

chmod 755 filename (所属者有所有的权限，而同组的人只有读的权限)

