# shadowsocks-Heroku-python
shadowsocks over WebSocket, support Heroku.

[![](https://www.herokucdn.com/deploy/button.svg)](https://heroku.com/deploy?template=https://github.com/onplus/shadowsocks-websocket-python/tree/deploy)

设置 加密算法和app 密码

![deploy](https://user-images.githubusercontent.com/31188782/31343896-ab0a868a-ad43-11e7-8a83-369cf5e385b0.jpg)

支持的加密算法类型如下https://github.com/mrluanma/shadowsocks-heroku#supported-ciphers

## 启动本地 Client（方法1）
1. 下载release https://github.com/onplus/shadowsocks-heroku/releases （[备份](https://github.com/onplus/archive/tree/master/tool)）
2. 修改config.json参数，运行ss-h.exe 或 start.vbs (或 [win托盘工具taskbar.exe](https://github.com/onplus/shadowsocks-heroku/issues/39))
5. 启动成功，命令行显示：`server listening at { address: '127.0.0.1', family: 'IPv4', port: 1080 }`



## 启动本地Client（方法2）[推荐！！！]

1、直接点击此链接下载[SSR(7Z)](https://raw.githubusercontent.com/GamerNoTitle/GamerNoTitle.github.io/master/files/SSR/ShadowsocksR-win-4.9.2.7z)或[SSR(ZIP)](https://raw.githubusercontent.com/GamerNoTitle/GamerNoTitle.github.io/master/files/SSR/ShadowsocksR-win-4.9.2.zip)或[SSTap(ZIP)](https://raw.githubusercontent.com/GamerNoTitle/GamerNoTitle.github.io/master/files/SSTap/SSTap-1.0.9.7.zip)

2、在SSR或SSTap中配置服务器（这里只提供SSR的配置方法）

![](https://github.com/GamerNoTitle/Picture-repo/blob/master/ss-on-heroku/SSR-config1.png?raw=true)

3、点确定即可

4、右键托盘小飞机，选到自己的服务器

![](https://github.com/GamerNoTitle/Picture-repo/blob/master/ss-on-heroku/SSR-Config2.jpg?raw=true)

5、最后在系统代理模式选择全局代理即可

## 配置代理（Chrome）

1. 下载：Chrome 浏览器 [SwitchyOmega](https://github.com/FelisCatus/SwitchyOmega/releases) 插件（[参考教程](https://github.com/FelisCatus/SwitchyOmega/wiki/GFWList), 导入备份文件[SSHeroku.Bak.zip](https://github.com/onplus/shadowsocks-heroku/files/1371313/SSHeroku.zip)）

2. 安装：打开浏览器的扩展程序页面 `chrome://extensions`，把 `SwitchyOmega.crx` 文件拖放到浏览器扩展程序页面安装 

3. 配置：添加SwitchyOmega代理服务器
```
    代理协议： SOCKS5
    代理服务器local_address：127.0.0.1 
    代理端口local_port： 1080 
```