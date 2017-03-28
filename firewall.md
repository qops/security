# Firewalld in centos 7

a new way to use iptables, don't use iptables any more.
http://www.firewalld.org/

## open a port

```
firewall-cmd --permanent --zone=public --add-port=80/tcp
firewall-cmd --permanent --zone=public --add-port=443/tcp
firewall-cmd --complete-reload
```

