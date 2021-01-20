
# vur
vur is a custom xbps-src repo / custom repo(with xbps binaries) that includes packages which can not be accepted into [void-packages](https://github.com/void-linux/void-packages/) or removed from it. 


## using this custom repo to install binaries 

1. sudo touch /etc/xbps.d/10-vur.conf <br><br>
2. put this in the file : repository=https://siduck76.github.io/VUR/generic/ <br><br>
Update your repos<br><br>
3. sudo xbps-install -S packagename

