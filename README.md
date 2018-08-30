1.服务端部署后，应 open app ，显示 Bad Request，表示部署成功。

2.客户端应使用websocket+tls传输协议。Vmess协议的 users id 应当换成自己的UUID，"alterId": 64

# v2ray 部署在 openshift starter
openshift: 内存设置为256M，每 project 可配置 4 Pods。
环境变量： CONFIG_JSON（配置）、CERT_PEM（证书）、KEY_PEM（私钥）

Docker 镜像：silentmx/openshift-v2ray
