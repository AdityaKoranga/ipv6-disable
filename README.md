# ipv6-disable
disabling the ipv6 support

```bash
sudo nano /etc/sysctl.conf
```

Add the following lines to the end of the file:
```bash
net.ipv6.conf.all.disable_ipv6 = 1
net.ipv6.conf.default.disable_ipv6 = 1
net.ipv6.conf.lo.disable_ipv6 = 1
```

Now final step:
```bash
sudo sysctl -p
```
