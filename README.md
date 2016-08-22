# files

# collectd

https://devops.profitbricks.com/tutorials/how-to-install-and-configure-collectd-and-collectd-web-to-monitor-a-centos-7-server/
```
sudo yum install epel-release
sudo yum --enablerepo=epel install collectd collectd-ping
sudo rm /etc/collectd.conf
sudo wget -O https://raw.githubusercontent.com/GBurg/files/master/collectd.conf /etc/collectd.conf
```

edit the /etc/collectd.conf file and change the hostname to something descriptive

```
sudo systemctl start collectd
sudo systemctl enable collectd
```
