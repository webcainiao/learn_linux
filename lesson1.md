# linux基础知识

标签    ： linux

---

1. 联网设置

$ ifconfig // 列出IP，mac,mask等信息。

$ vim /etc/sysconfig/network-scripts/xxxxxx(网络配置文件)
修改ONBOOT=yes,然后重启网络：

$ service network restart //centos6，centos7略不同

2.防火墙
centos6
```
$ service iptables status
$ service iptables stop
```
centos7
```
$ systemctl stop firewalld.service
```



