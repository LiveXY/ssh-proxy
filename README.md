ssh-proxy
======
安装方法：
```
git clone https://github.com/LiveXY/ssh-proxy.git
cd ssh-proxy
npm install -ddd && npm link
```
使用方法：
```
sshproxy list/start/stop/restart/state/set/add/del/clear [options]

实例：
sshproxy list	 查看所有SSH代理服务器信息
sshproxy start	 启动默认的SSH代理服务器
sshproxy stop	 停止SSH代理服务器
sshproxy restart 重启SSH代理服务器
sshproxy state	 查看SSH代理服务器是否启动

sshproxy add -i ssh1 -h host -P port -u user -p password
添加SSH代理服务器，-P默认22、-u默认root

sshproxy del -i ssh1		 删除SSH代理服务器ssh1
sshproxy set -i ssh1 -P port 配置默认使用服务器和绑定端口，默认7070
sshproxy clear			 	 清理使用SSH代理服务器

```
可使用在MAC和LINUX系统下