## Advertisement
<a href="https://www.huobi.be/zh-cn/topic/invited/?invite_code=qpi54">
<img width="auto" height="100" src="/doc/images/zanzhu-1.png"/>
</a>

## GOPROXY Introduction
<img src="https://github.com/snail007/goproxy/blob/master/doc/images/logo.jpg?raw=true" width="200" height="auto"/>
The GoProxy is a high-performance http proxy, https proxy, socks5 proxy, ss proxy, websocket proxies, tcp proxies, udp proxies,  game shield, game proxies. Support forward proxies, reverse proxy, transparent proxy, internet nat proxies, https proxy load balancing, http proxy load balancing , socks5 proxies load balancing, socket proxy load balancing, ss proxy load balancing, TCP / UDP port mapping, SSH transit, TLS encrypted transmission, protocol conversion, anti-pollution DNS proxy, API authentication, speed limit, limit connection. Reverse proxies to help you expose a local server behind a NAT or firewall to the internet so that you or your visitors can access it directly and easily. 

---

[![stable](https://img.shields.io/badge/stable-stable-green.svg)](https://github.com/snail007/goproxy/) [![license](https://img.shields.io/github/license/snail007/goproxy.svg?style=plastic)]() [![download_count](https://img.shields.io/github/downloads/snail007/goproxy/total.svg?style=plastic)](https://github.com/snail007/goproxy/releases) [![download](https://img.shields.io/github/release/snail007/goproxy.svg?style=plastic)](https://github.com/snail007/goproxy/releases) 

---

### [点击我观看视频教程](https://space.bilibili.com/472844633)
- [中文介绍（必看）](https://github.com/snail007/goproxy/blob/master/README_ZH.md)
- [下载地址（国外）](https://github.com/snail007/goproxy/releases)
- [下载地址（国内）](https://mirrors.host900.com/snail007/goproxy/)
- [官方手册（国外）](https://snail007.github.io/goproxy/manual/zh/)
- [官方手册（国内）](https://snail.gitee.io/proxy/manual/zh/)
- [Download](https://github.com/snail007/goproxy/releases)
- [Desktop Edition, Web Console : ProxyAdmin](https://github.com/snail007/proxy_admin_free)
- [Android Global Proxy Edition](https://github.com/snail007/goproxy-ss-plugin-android) 
- [Android Proxy Server Edition](https://github.com/snail007/goproxy-android) 
- [SDK](https://github.com/snail007/goproxy-sdk)
- [GORPOXY Manual](https://snail007.github.io/goproxy/manual/)
- [GORPOXY Tutorial](https://snail007.github.io/goproxy)
- [Free version VS commercial version](https://snail007.github.io/goproxy/page/free_vs_commercial/)

### ProxyAdmin Demo
And ProxyAdmin is a powerful web console of snail007/goproxy .

![](https://github.com/snail007/proxy_admin_free/raw/master/res/images/socks5_en.gif)

### What can it do?
- Chained proxies, the program itself can be used as an proxies, and if it is set up, it can be used as a secondary proxies or even an N-level proxies.
- Communication encryption, if the program is not a level one proxies, and the upper level proxies is also the program, then the communication between the upper level proxies and the upper level proxies can be encrypted, and the underlying tls high-intensity encryption is used, and the security is featureless.
- Smart HTTP, SOCKS5 proxy, will automatically determine whether the visited website is blocked. If it is blocked, it will use the upstream proxies (provided that the upstream proxies is configured) to access the website; if the visited website is not blocked, in order to speed up the access, the proxies will Direct access to the website without using a upstream proxies.
- Domain name black and white list, more free to control the way the website is accessed.
- Cross-platform, whether you are widows, linux, mac, or even raspberry pie, you can run the proxy very well.
- Multi-protocol support, support for HTTP(S), TCP, UDP, Websocket, SOCKS5 proxy.
- TCP/UDP port forwarding.
- Support intranet penetration, protocol supports TCP and UDP.
- SSH relay, HTTP (S), SOCKS5 proxy supports SSH relay, the upper Linux server does not need any server, a local proxy can be happy online.
- [KCP](https://github.com/xtaci/kcp-go) protocol support, HTTP(S), SOCKS5, SPS proxy supports KCP protocol to transmit data, reduce latency and improve browsing experience.
- Dynamic selection of upstream proxies, through the external API, HTTP (S), SOCKS5, SPS proxies can achieve user-based or IP-based speed limit, connection limit, dynamic access to upstream.
- Flexible upstream allocation, HTTP(S), SOCKS5 proxy can implement user- or IP-based speed limit, connection limit, and upper-level through configuration files.
- Transparent HTTP (S) proxy, in conjunction with iptables, forwards the outgoing 80, 443 traffic directly to the proxy at the gateway, enabling non-aware intelligent router proxy.
- Protocol conversion, which can convert existing HTTP(S) or SOCKS5 or SS proxy into one port and support HTTP(S) and SOCKS5 and SS proxy at the same time. Converted SOCKS5 and SS proxy. If the upstream is SOCKS5 proxy, then UDP is supported. Features while supporting powerful cascading authentication.
- Custom underlying encrypted transmission, http(s)\sps\socks proxy can encrypt tcp data via tls standard encryption and kcp protocol on top of tcp, in addition to support custom encryption after tls and kcp, that is Said custom encryption and tls|kcp can be used in combination, the internal AES256 encryption, you only need to define a password when you use it.
- Underlying compression efficient transmission, http(s)\sps\socks proxy can encrypt tcp data through custom encryption and tls standard encryption and kcp protocol on tcp, and can also compress data after encryption, that is, compression function And custom encryption and tls|kcp can be used in combination.
- Secure DNS proxy, which can secure and prevent pollution DNS queries through encrypted proxy communication between the DNS proxy server provided by the local proxy and the upstream proxy.
- Load balancing, high availability, HTTP(S)\SOCKS5\SPS proxies supports upstream load balancing and high availability, and multiple upstream repeat-P parameters can be used.
- Specify the egress IP. The HTTP(S)\SOCKS5\SPS\TCP proxy supports the client to connect with the ingress IP, and uses the ingress IP as the egress IP to access the target website. If the ingress IP is an intranet IP, the egress IP does not use the ingress IP.
- Support speed limit, HTTP(S)\SOCKS5\SPS\TCP proxy supports speed limit.
- SOCKS5 proxies supports cascading certification.
- The certificate parameter uses base64 data. By default, the -C, -K parameter is the path of the crt certificate and the key file. If it is the beginning of base64://, then the latter data is considered to be base64 encoded and will be used after decoding.
- Support client IP black and white list, more secure control of client access to proxy service, if black and white list is set at the same time, then only whitelist is effective. Socks / HTTP(S) / SPS / TCP / UDP / DNS / intranet NAT The bridge/intranet NAT the tbridge and supports the client IP black and white list.
- Range ports listen on, HTTP(S)\SOCKS5\SPS\TCP proxy supports port range listening, avoiding starting too many processes and improving performance.

### Why do you need it?

- When for some reason we are unable to access our services elsewhere, we can establish a secure tunnel to access our services through multiple connected proxy nodes.
- WeChat interface is developed locally for easy debugging.
- Remote access to intranet machines.
- Play LAN games with your friends.
- I used to play only on the LAN, and now I can play anywhere.
- Replace the sword inside Netnet, show IP internal Netcom, peanut shell and other tools.
- ..

 
The manual on this page applies to the latest version of goproxy. Other versions may not be applicable. Please use the command according to your own instructions.
 

### Joining the organization
[Click to join the gitter](https://gitter.im/go-proxy/Lobby?utm_source=share-link&utm_medium=link&utm_campaign=share-link)

[Click to join the TG](https://t.me/snail007_goproxy)

## Download and install 

### Quick installation

0. If your VPS is a Linux 64-bit system, you only need to execute the following sentence to complete the automatic installation and configuration.

Tip: All operations require root privileges.

The free version performs this:

```shell
curl -L https://raw.githubusercontent.com/snail007/goproxy/master/install_auto.sh | bash
```

The commercial version performs this:

```shell
curl -L https://raw.githubusercontent.com/snail007/goproxy/master/install_auto_commercial.sh | bash
```

The installation is complete, the configuration directory is /etc/proxy. For more detailed usage, please refer to the manual directory above to learn more about the features you want to use.
If the installation fails or your vps is not a linux64-bit system, follow the semi-automatic steps below to install:
  
### Manual installation

1. Download the proxy

Download address: https://github.com/snail007/goproxy/releases/latest

Let's take v7.9 as an example. If you have the latest version, please use the latest version of the link. Note that the version number in the download link below is the latest version number.

The free version performs this:

```shell
cd /root/proxy/
wget https://github.com/snail007/goproxy/releases/download/v8.7/proxy-linux-amd64.tar.gz
```

The commercial version performs this:

```shell
cd /root/proxy/
wget https://github.com/snail007/goproxy/releases/download/v7.9/proxy-linux-amd64_commercial.tar.gz
```

2. Download the automatic installation script

The free version performs this:

```shell
cd /root/proxy/
wget https://raw.githubusercontent.com/snail007/goproxy/master/install.sh
chmod +x install.sh
./install.sh
```

The commercial version performs this:

```shell
cd /root/proxy/
wget https://raw.githubusercontent.com/snail007/goproxy/master/install_commercial.sh
chmod +x install_commercial.sh
./install_commercial.sh
```

## TODO
- http,socks proxy multiple upstream load balancing?
- http(s) proxy to increase pac support?
- Welcome to add group feedback..

## License
Proxy is licensed under GPLv3 license.

## Contact
Official QQ exchange group: 42805407

## Donation
If the proxy helps you solve a lot of problems, you can better support the proxy through the donation below.

BTC  ADDRESS: `1BJcBhGhREiz1q3VTYoiVPuAZy5PGxRG9z`

<img src="https://raw.githubusercontent.com/snail007/goproxy/master/docs/img/btc.png" width="150" height="auto"/>  

ETH  ADDRESS: `0x0fA4c567768d2E59E6221152EA52F4842866AFC8`

<img src="https://raw.githubusercontent.com/snail007/goproxy/master/docs/img/eth.png" width="150" height="auto"/>  

### Source code declaration

The author of this project found that a large number of developers based on the project for secondary development or using a large number of core code of the project without complying with the GPLv3 agreement, which seriously violates the original intention of using the GPLv3 open source agreement in this project. In view of this situation, the project adopts the source. The code delays the release strategy, to a certain extent, to curb these behaviors that do not respect open source and do not respect the labor results of others.
This project will continue to update the iterations and continue to release the full platform binary program, providing you with powerful and convenient proxies tools.
If you have customized, business needs, please send an email to `arraykeys@gmail.com`