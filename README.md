甲骨文云dd重装系统一键脚本，轻松拯救玩坏的小鸡！
- 四月 11, 2022
目前是会员专享视频，4月17日公开发布！

https://youtu.be/FhuneE1BfaI














几个情况需要重装系统

1.我的VPS装了一堆东西，很乱，想还原

2.我的VPS之前东西和现在要装的东西冲突了。无法进行安装了

3.我的VPS被人侵入当矿机了，机器满负荷运载

4.想尝试bbr其他版本，ARM目前还是会失联

5.更纯净更稳定

最关键是甲骨文云你删机不一定能开出新机！所以重装系统很重要！





重装前的故事背景

甲骨文云ARM或者AMD架构，Ubuntu系统

几分钟内dd成debian或者ubuntu

群友分享的，他经常用。我也成功重装了！





1.一键脚本

```
bash <(wget --no-check-certificate -qO- 'https://moeclub.org/attachment/LinuxShell/InstallNET.sh') -d 10 -v 64 -a -firmware -p 12345
```



系统参数

-d 10  【7、8、9、10】Debian

-u 20.04  【14.04、16.04、18.04、20.04】Ubuntu



密码参数，可以改成别的

-p 12345





2.刚开始，都是自动的等


















3.这就结束了


















重装后3分钟VPS自动重启，



4.用户名root





5.密码就是你自己设置的12345或者别的








6.好了直接重装完了，直接root权限了，又可以愉快的玩耍了！










这时候想改root账户对的密码输入以下命令，输入时密码不显示，感觉像是没输进去，正常盲打即可！输入两次！

passwd




这个系统装BBR前先走这个命令

apt update -y && apt install -y curl && apt install -y socat && apt install wget -y



BBR PLUS 四合一脚本

wget -N --no-check-certificate "https://raw.githubusercontent.com/chiakge/Linux-NetSpeed/master/tcp.sh" && chmod +x tcp.sh && ./tcp.sh
