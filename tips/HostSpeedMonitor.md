# 路由下主机数据传输速率查看程序命令

![1](https://user-images.githubusercontent.com/73426989/150641844-182e6054-b757-457a-b6a8-73a40151519b.jpg)           

路由下主机数据传输速率查看程序命令： 

```
iftop -i br-lan
```

如果你使用的固件没有预装此程序，那么一般情况下固件自带的软件源都发行有iftop，可以通过opkg安装即可，依次执行以下两条命令：               

```
opkg update
opkg install iftop
```

然后再尝试运行命令：     

```
iftop -i br-lan
```

如图所示，此软件第一行是自动调整刻度的标尺，白色长条就是直观图形显示某主机的出或进速率。          

第二列是所有内网主机，第一列是公网上和此主机通信的服务器的IP。               

第三列是精确的数值显示，三个数, 分别表示最近的2s, 10s, 40s的平均流量。             


[返回主页](https://boduoyejieyi666.github.io/whonolikeboduoyejieyi/)           


