# DockerShadowsocksServer

几行命令行搭建shadowsocks server

1. 安装最基础的docker: apt-get install docker; yum install docker
2. docker pull shadowsocks/shadowsocks-libev
3. docker run -e PASSWORD=helloworld -e METHOD=aes-128-cfb -p22360:8388 -p22360:8388/udp -d shadowsocks/shadowsocks-libev

其中helloworld是密码，22360是对外端口 -p后面没有空格，aes-128-cfb是加密算法，用其他算法速度明显变慢，经过测试这个是最快的。不管不问稳定运行半年没问题。

<img width="150" alt="WechatIMG151" src="https://user-images.githubusercontent.com/2038071/110611311-0f008000-81ca-11eb-97b4-18fb7aa1d941.png">
