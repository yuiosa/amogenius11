# mogenius11


######################

8. 客户端配置如下所示

V2ray

```
地址：xxx-xxx.koyeb.app 或 CF优选IP
端口：443
默认UUID：24b4b1e1-7a89-45f6-858c-242cf53b5bdb
vmess额外id：0
加密：none
传输协议：ws
伪装类型：none
伪装域名：xxx-xxx.koyeb.app
路径：/24b4b1e1-7a89-45f6-858c-242cf53b5bdb-vless
vless使用(/自定义UUID码-vless)，vmess使用(/自定义UUID码-vmess)
底层传输安全：tls
跳过证书验证：false
```

Trojan-go

```bash
{
    "run_type": "client",
    "local_addr": "127.0.0.1",
    "local_port": 1080,
    "remote_addr": "xxx-xxx.koyeb.app",
    "remote_port": 443,
    "password": [
        "24b4b1e1-7a89-45f6-858c-242cf53b5bdb"
    ],
    "websocket": {
        "enabled": true,
        "path": "/24b4b1e1-7a89-45f6-858c-242cf53b5bdb-trojan",
        "host": "xxx-xxx.koyeb.app"
    }
}
```

ShadowSocks

```bash
服务器地址: xxx-xxx.koyeb.app
端口: 443
密码：24b4b1e1-7a89-45f6-858c-242cf53b5bdb
加密：chacha20-ietf-poly1305
插件程序：xray-plugin_windows_amd64.exe
说明：需将插件 https://github.com/shadowsocks/xray-plugin/releases 下载解压后放至shadowsocks同目录
插件选项: tls;host=xxx-xxx.koyeb.app;path=/24b4b1e1-7a89-45f6-858c-242cf53b5bdb-ss
```

## 注意
