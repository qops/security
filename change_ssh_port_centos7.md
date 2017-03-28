# Change Default SSH Port


## Install Dependencies
```
yum install policycoreutils-python
```
## SELinux
```
semanage port -a -t ssh_port_t -p tcp 6666

```

## Change SSH Config, Port
```
# vim /etc/ssh/sshd_config
Port 6666
```

## Firewalld Open
```
firewall-cmd --permanent --zone=public --add-port=6666/tcp
firewall-cmd --complete-reload
```

## Restart sshd
```
systemctl restart sshd
```

## Check
```
netstat -tulpn
telnet server_ip 6666
```
