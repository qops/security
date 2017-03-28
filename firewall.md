# Firewalld in CentOS 7

a new way to use iptables, don't use iptables any more.

http://www.firewalld.org/

## Enable and Disable

http://www.firewalld.org/documentation/howto/enable-and-disable-firewalld.html

## Open a Port

```
firewall-cmd --permanent --zone=public --add-port=80/tcp
firewall-cmd --permanent --zone=public --add-port=443/tcp
firewall-cmd --complete-reload
```

