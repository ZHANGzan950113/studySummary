# study Summary

documenting my learning life

## Vue

## Cloud sever

### question
#### RNING! The remote SSH server rejected X11 forwarding request.

远程 SSH 服务器拒绝了 X11 转发请求。

**安装x11依赖库**

```
sudo yum install xauth x11-apps
```

### mysql

yum不存在mysql安装包。需要先手动添加。

```powershell
sudo rpm -Uvh https://dev.mysql.com/get/mysql80-community-release-el7-5.noarch.rpm
```

然后安装

```shell
sudo yum -y install mysql-community-server --enablerepo=mysql80-community --nogpgcheck
```

```shell
mysql -V 检查安装结果
```

安装完mysql，需要进行配置

```powershell
sudo systemctl start mysqld 启动
sudo systemctl enable mysqld 开机运行
sudo systemctl status mysqld 程序状态
```

获取初始密码

```shell
sudo grep 'temporary password' /var/log/mysqld.log
```

对mysql配置

```powershell
sudo mysql_secure_installation
```

### VMware



