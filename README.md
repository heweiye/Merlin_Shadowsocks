# Shadowsocks客户端离线安装包 for Merlin梅林固件
该SS客户端集成了SS&SSR&kcptun
<br>version文件记录了各版本的md5信息
偶数版本较稳定, 3.60为官方最后一个版本,3.6.01是 民间修改 增加了对chain_a的支持
# 安装
请开启jfs后 根据软件中心离线安装的提示安装，如无法正常安装 可SSH硬装 以SSH安装3.6.0为例:
<br>cd /tmp
<br>wget -N -O shadowsocks.tar.gz https://raw.githubusercontent.com/heweiye/Merlin_Shadowsocks/master/shadowsocks_3.6.0.tar.gz
<br>tar -zxvf /tmp/shadowsocks.tar.gz
<br>chmod +x /tmp/shadowsocks/install.sh
<br>sh /tmp/shadowsocks/install.sh
