# Shadowsocks客户端离线安装包 for Merlin梅林固件
该SS客户端集成了SS&SSR&kcptun
<br>version文件记录了各版本的md5信息
偶数版本较稳定, 3.60为官方最后一个版本,3.6.01是 民间修改 增加了对chain_a的支持
# 安装
请开启jfs后 根据软件中心离线安装的提示安装，如无法正常安装 可SSH硬装 以SSH安装3.6.0为例:
```Bash
cd /tmp
wget -N -O shadowsocks.tar.gz https://raw.githubusercontent.com/heweiye/Merlin_Shadowsocks/master/shadowsocks_3.6.0.tar.gz
tar -zxvf /tmp/shadowsocks.tar.gz
chmod +x /tmp/shadowsocks/install.sh
sh /tmp/shadowsocks/install.sh
```
<br>部分验证固件版本导致无法安装的可以修改编辑
/tmp/shadowsocks/install.sh文件
找到if [ "$firmware_comp" == "-1" ];then
修改为if [ "$firmware_comp" == "1" ];then

