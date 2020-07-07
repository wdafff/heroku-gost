[![Deploy](https://www.herokucdn.com/deploy/button.png)](https://heroku.com/deploy)  
  
> 提醒： 滥用可能导致账户就被BAN！！！  
  
###### 点击图标部署项目：  
  
1. 变量 METHOD 如不需要，保持默认留空即可，自定义使用方式参考 https://github.com/ginuerzh/gost/ https://docs.ginuerzh.xyz/gost/  
  
2. 完成部署后，打开app ，显示404 page not found，表示部署成功  
  
###### 客户端使用，这里介绍如下二种方式
  
* v2ray ws tls: 
```bash
{
            "protocol": "socks",
            "tag": "herokuapp",
            "settings": {"servers": [{"address": "xxxxxxxxx.herokuapp.com": 443}]},
            "streamSettings": {"network": "ws","security": "tls","tlsSettings": {"allowInsecure": false,"serverName": "xxxxxxxxx.herokuapp.com"},"wsSettings": {"path": "/ws","headers": {"Host": "xxxxxxxxx.herokuapp.com"}}}
}
```
  
* gost -L=:1080 -F=socks5+wss://xxxxxxxxx.herokuapp.com:443
  
###### 搭配clouflare cdn
* 参考https://github.com/CCChieh/IBMYes#cloudflare-%E9%AB%98%E9%80%9F%E8%8A%82%E7%82%B9%E4%B8%AD%E8%BD%AC
