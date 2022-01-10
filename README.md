# VPS自动配置内容

1. 配置基础环境: 包括终端字符集、基本工具vim/git/python3.9+等
2. 配置shell环境： 新建工作目录，增加普通用户,使用 `oh-my-zsh`


## iptables防火墙配置脚本

如果使用`iptables`配置防火墙规则，那么可以使用本脚本来管理防火墙规则。


```
Usage:
    fwctl <init|save|restore>
     firewall manager| 防火墙管理脚本

Description:
    init    第一次初始化防火墙规则，白名单为空
    save    导出防火墙规则及白名单ipset列表
    restore 恢复防火墙规则及白名单ipset列表
    status  查看防火墙状态规则

    add_port 添加开放TCP端口 
    add_wip  添加白名单IP
    del_port 删除开放TCP端口 
    del_wip  删除白名单IP

```


## VPS配置管理脚本
> 购买VPS后，可以使用此脚本配置初始化环境、安装python、curl、设置时区、中文字符集支持等功能。

使用帮助信息：

```
vpsctl -h
```


---
