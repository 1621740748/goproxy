## 赞助商广告
<a href="https://www.huobi.be/zh-cn/topic/invited/?invite_code=qpi54">
<img width="auto" height="100" src="/doc/images/zanzhu-1.png"/>
</a>

## GOPROXY简介
<img src="/doc/images/logo.jpg" width="200" height="auto"/>  
一款轻量级、功能强大、高性能的http代理、https代理、socks5代理、内网穿透代理服务器、ss代理、游戏盾、游戏代理，支持API代理认证。websocke代理、tcp代理、udp代理、socket代理、高防服务器。支持正向代理、反向代理、透明代理、TCP内网穿透、UDP内网穿透、HTTP内网穿透、HTTPS内网穿透、https代理负载均衡、http代理负载均衡、socks5代理负载均衡、socket代理负载均衡、ss代理负载均衡、TCP/UDP端口映射、SSH中转、TLS加密传输、协议转换、防污染DNS代理，限速，限连接数。官方QQ交流群: 42805407。 

---

[![stable](https://img.shields.io/badge/stable-stable-green.svg)](https://github.com/snail007/goproxy/) [![license](https://img.shields.io/github/license/snail007/goproxy.svg?style=plastic)]() [![download_count](https://img.shields.io/github/downloads/snail007/goproxy/total.svg?style=plastic)](https://github.com/snail007/goproxy/releases) [![download](https://img.shields.io/github/release/snail007/goproxy.svg?style=plastic)](https://github.com/snail007/goproxy/releases)  

---
### [点击我观看视频教程](https://space.bilibili.com/472844633)
- [下载地址（国外）](https://github.com/snail007/goproxy/releases)
- [下载地址（国内）](https://mirrors.host900.com/snail007/goproxy/)
- [官方手册（国外）](https://snail007.github.io/goproxy/manual/zh/)
- [官方手册（国内）](https://snail.gitee.io/proxy/manual/zh/)
- [桌面版，控制面板ProxyAdmin](https://github.com/snail007/proxy_admin_free/blob/master/README_ZH.md)
- [安卓全局代理版](https://github.com/snail007/goproxy-ss-plugin-android) 
- [安卓全能代理版](https://github.com/snail007/goproxy-android) 
- [安卓内网穿透客户端](https://github.com/snail007/lanass) 
- [SDK](https://github.com/snail007/goproxy-sdk)
- [GORPOXY实战教程](https://snail007.github.io/goproxy)  
- [免费版VS商业版(安装、激活)](https://snail007.github.io/goproxy/page/free_vs_commercial/)

## ProxyAdmin介绍预览（这不是goproxy，是控制面板友情链接；安装使用goproxy请往下看，谢谢！）
`ProxyAdmin` 是强大的代理服务工具 snail007/goproxy 的控制面板，运行了它，一秒让你的服务器变为强大的代理服务器，友好的交互界面，小白也能轻松上手，让你用起来得心应手，心情舒畅。

![](https://github.com/snail007/proxy_admin_free/raw/master/res/images/socks5_cn.gif)

### goproxy能干什么？
- 链式代理，程序本身可以作为一级代理，如果设置了上级代理那么可以作为二级代理，乃至N级代理。  
- 通讯加密，如果程序不是一级代理，而且上级代理也是本程序，那么可以加密和上级代理之间的通讯，采用底层tls高强度加密，安全无特征。  
- 智能HTTP代理，HTTPS代理，SOCKS5代理，会自动判断访问的网站是否屏蔽，如果被屏蔽那么就会使用上级代理(前提是配置了上级代理)访问网站;如果访问的网站没有被屏蔽，为了加速访问，代理会直接访问网站，不使用上级代理。  
- 域名黑白名单，更加自由的控制网站的访问方式。  
- 跨平台性，无论你是widows，linux，还是mac，甚至是树莓派，都可以很好的运行proxy。  
- 多协议支持，支持HTTP(S)，TCP，UDP，Websocket，SOCKS5代理。  
- TCP/UDP端口转发。 
- 游戏盾，游戏代理，高防服务器。 
- 内网穿透，P2P传输，协议支持TCP和UDP，针对HTTP的优化穿透。  
- SSH中转，HTTP(S)，SOCKS5代理支持SSH中转，上级Linux服务器不需要任何服务端，本地一个proxy即可开心上网。  
- [KCP](https://github.com/xtaci/kcp-go)协议支持，HTTP(S)，SOCKS5代理支持KCP协议传输数据，降低延迟，提升浏览体验。  
- 动态选择上级代理，通过外部API，HTTP(S)，SOCKS5，SPS代理可以实现基于用户或者IP的限速，连接数限制，动态获取上级。
- 灵活的上级分配，HTTP(S)，SOCKS5，SPS代理可以通过配置文件实现基于用户或者IP的限速，连接数限制，指定上级。
- 反向代理，支持直接把域名解析到proxy监听的ip，然后proxy就会帮你代理访问需要访问的HTTP(S)网站。  
- 透明HTTP(S)代理，配合iptables，在网关直接把出去的80，443方向的流量转发到proxy，就能实现无感知的智能路由器代理。  
- 协议转换，可以把已经存在的HTTP(S)或SOCKS5或SS代理转换为一个端口同时支持HTTP(S)和SOCKS5和SS代理，转换后的SOCKS5和SS代理如果上级是SOCKS5代理，那么支持UDP功能，同时支持强大的级联认证功能。
- 自定义底层加密传输，http(s)\sps\socks代理在tcp之上可以通过tls标准加密以及kcp协议加密tcp数据，除此之外还支持在tls和kcp之后进行自定义加密，也就是说自定义加密和tls|kcp是可以联合使用的，内部采用AES256加密，使用的时候只需要自己定义一个密码即可。
- 底层压缩高效传输，http(s)\sps\socks代理在tcp之上可以通过自定义加密和tls标准加密以及kcp协议加密tcp数据，在加密之后还可以对数据进行压缩，也就是说压缩功能和自定义加密和tls|kcp是可以联合使用的。
- 安全的DNS代理，可以通过本地的proxy提供的DNS代理服务器与上级代理加密通讯实现安全防污染的DNS查询。
- 负载均衡，高可用，HTTP(S)\SOCKS5\SPS代理支持上级负载均衡和高可用，多个上级重复-P参数即可。  
- 指定出口IP，HTTP(S)\SOCKS5\SPS代理支持客户端用入口IP连接过来的，就用入口IP作为出口IP访问目标网站的功能。如果入口IP是内网IP，出口IP不会使用入口IP
- 支持限速，HTTP(S)\SOCKS5\SPS\TCP代理支持限速。  
- 支持限连接数，HTTP(S)\SOCKS5\SPS\TCP代理支持限连接数。  
- SOCKS5代理支持级联认证。  
- 证书参数使用base64数据，默认情况下-C，-K参数是crt证书和key文件的路径，如果是base64://开头，那么就认为后面的数据是base64编码的，会解码后使用。  
- 支持客户端IP黑白名单，更加安全的控制客户端对代理服务的访问，如果黑白名单同时设置，那么只有白名单生效。socks/http(s)/sps/tcp/udp/dns/内网穿透bridge/内网穿透tbridge，都支持客户端IP黑白名单。 
- 端口范围批量监听，HTTP(S)\SOCKS5\SPS\TCP代理支持指定端口范围监听，避免启动过多进程，提高性能。

### 为什么需要它？

- 当由于某某原因，我们不能访问我们在其它地方的服务，我们可以通过多个相连的proxy节点建立起一个安全的隧道访问我们的服务。  
- 微信接口本地开发，方便调试。  
- 远程访问内网机器。  
- 和小伙伴一起玩局域网游戏。  
- 以前只能在局域网玩的，现在可以在任何地方玩。  
- 替代圣剑内网通，显IP内网通，花生壳之类的工具。 
- 有大量IP资源，想变现，对外提供IP代理服务。 
- 有大量拨号VPS，想对外提供IP代理服务。
- 公司安全要求，审计员工对互联网的访问。
- 想要一个高性能稳定的，认证功能齐全的代理服务。
- 想一个固定入口，实现动态IP出口。
- ..。  

 
本页手册适用于最新版goproxy，其他版本可能有的地方不再适用，请自己根据命令帮助使用。  
 

### 加入组织  
[点击加入交流组织gitter](https://gitter.im/go-proxy/Lobby?utm_source=share-link&utm_medium=link&utm_campaign=share-link)  

[点击加入交流组织TG](https://t.me/snail007_goproxy)  

## 下载安装 goproxy

### 快速安装 goproxy

如果你的VPS是linux64位的系统，那么只需要执行下面一句，就可以完成自动安装和配置.

提示:所有操作需要root权限。 

免费版执行这个：  

```shell  
curl -L https://mirrors.host900.com/snail007/goproxy/install_auto.sh | bash  
```  

商业版执行这个：  

```shell  
curl -L https://mirrors.host900.com/snail007/goproxy/install_auto_commercial.sh | bash  
```  

安装完成，配置目录是/etc/proxy，更详细的使用方法请参考上面的手册目录，进一步了解你想要使用的功能。  
如果安装失败或者你的vps不是linux64位系统，请按照下面的半自动步骤安装:  
  
### 手动安装 goproxy

1.下载goproxy

根据你的平台和CPU类型选择,下载地址: https://mirrors.host900.com/snail007/goproxy ,  

这里以`proxy-linux-amd64.tar.gz`为例,具体使用的时候,请根据你的平台和CPU类型选择具体文件名称.   

免费版执行这个：  

```shell  
cd /root/proxy/  
wget https://mirrors.host900.com/snail007/goproxy/proxy-linux-amd64.tar.gz  
```  

商业版执行这个：  

```shell  
cd /root/proxy/  
wget https://mirrors.host900.com/snail007/goproxy/proxy-linux-amd64_commercial.tar.gz  
```  

2.下载自动安装脚本

免费版执行这个：  

```shell  
cd /root/proxy/  
wget https://raw.githubusercontent.com/snail007/goproxy/master/install.sh  
chmod +x install.sh  
./install.sh  
```  

商业版执行这个：  

```shell  
cd /root/proxy/  
wget https://raw.githubusercontent.com/snail007/goproxy/master/install_commercial.sh  
chmod +x install_commercial.sh  
./install_commercial.sh  
```  

## TODO  
- http，socks代理多个上级负载均衡?
- http(s)代理增加pac支持?
- 欢迎加群反馈..。  

## License  
Proxy is licensed under GPLv3 license。  

## Contact  
官方QQ交流群: 42805407  

## Donation  
如果proxy帮助你解决了很多问题，你可以通过下面的捐赠更好的支持proxy。  
<img src="/doc/images/alipay.jpg" width="200"  height="auto"/>  
<img src="/doc/images/wxpay.jpg" width="200"  height="auto"/>  

### 源代码申明

本项目作者发现大量的开发者基于本项目进行二次开发或使用大量本项目核心代码而不遵循GPLv3协议，这严重违背了本项目使用GPLv3开源协议的初衷，鉴于这种情况，本项目采取源代码延迟发布策略，在一定程度上遏制这些不尊重开源，不尊重他人劳动成果的行为。  
本项目会持续更新迭代，持续发布全平台的二进制程序，给大家提供强大便捷的代理工具。  
如果你有定制，商业需求请发邮件至`arraykeys@gmail.com`