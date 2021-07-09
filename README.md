

群主的ssr被封了，现在用Brook，配置方便操作简单。

[Brook服务端配置](https://txthinking.github.io/brook/#/zh-cn/brook-server)

[Brook客户端配置](https://txthinking.github.io/brook/#/zh-cn/install-gui-client)

# Deprecated
# DockerShadowsocksServer

几行命令行搭建shadowsocks server

1. 安装最基础的docker:yum install docker; apt-get install docker
2. docker pull shadowsocks/shadowsocks-libev
3. docker run -e PASSWORD=helloworld -e METHOD=aes-128-cfb -p22360:8388 -p22360:8388/udp -d shadowsocks/shadowsocks-libev

其中helloworld是密码，22360是对外端口 -p后面没有空格，aes-128-cfb是加密算法，用其他算法速度明显变慢，经过测试这个是最快的。不管不问稳定运行半年没问题。

客户端配置:

<img width="150" alt="WechatIMG151" src="https://user-images.githubusercontent.com/2038071/110611311-0f008000-81ca-11eb-97b4-18fb7aa1d941.png">


ps:租服务不要租那种有宽带上限的(1m带宽2m带宽没法用，大一点的奇贵)，租那种1一个月500G或者1T流量的无峰值上限的。一年参考价格300-600rmb足够n人使用，多几个人少几个人没感觉。群主使用的是搬瓦工。
