## 私人VPN
[参考](https://github.com/yukaiji/buildVpn)  
登录[vultr](www.vultr.com)新建服务器。  
添加服务器，纽约，选择最便宜价格(3.5$)，选择centos7se。  
取消底下的所有附加购买内容，确定为3.5$后购买。  
用Ping软件测试ip连接。  
用ip、用户名与密码在Termius软件登录。

部署VPN:
```zsh
wget --no-check-certificate https://raw.githubusercontent.com/teddysun/shadowsocks_install/master/shadowsocksR.sh
```
```zsh
chmod +x shadowsocksR.sh
```
```zsh
./shadowsocksR.sh 2>&1 | tee shadowsocksR.log
```

BBR加速
```zsh
wget --no-check-certificate https://github.com/teddysun/across/raw/master/bbr.sh
```
```zsh
chmod +x bbr.sh
```
```zsh
./bbr.sh
```

使用Shadowrocket连接
