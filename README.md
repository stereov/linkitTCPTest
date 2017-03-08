# linkitTCPTest
(1) 新建example application，选择Network_BSD_TCPServer<br>
(2) 修改.C文件中的ssid及密码<br>
![github](https://github.com/stereov/linkitTCPTest/raw/master/image/wlan_config.PNG)  <br>
(3) 连接2502开发板，打开Monitor，build application，下载到开发板 <br>
(4) 在monitor中查看wlan的连接状态，连接成功可以在monitor中查看ip，也可以在路由器中查看<br>
(5) 打开TCP调试软件(我用的是USR-TCP232)，填入开发板的ip，并设置为TCP Client,并连接<br>
(6) 调试软件连接成功后，发送任意内容给开发板，开发板会回复预定的内容，例子给的是“Hello Client” <br>
![github](https://github.com/stereov/linkitTCPTest/raw/master/image/results.PNG)  <br>
我看来下代码，这个连接是单次的，开发板回复后会自动关闭socket，可以按自己要求修改，也可以加入LCD显示。
