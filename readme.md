### 介绍
开发一个小程序项目有连接两台MQTT服务器的需求，试了[paho.mqtt.wxapp](https://github.com/tennessine/paho.mqtt.wxapp)和[MQTT.js](https://github.com/mqttjs/MQTT.js)两个适配微信的MQTT库，发现不能满足这个需求。看了下MQTT.js的源代码，发现它已经适配了微信基础库v1.7之后的WebScoket代码（最多连接5条ws），放弃改动。而paho.mqtt.wxapp这个库，还是用v1.7之前的代码，我就把WebSocket相关的API换成最新的，可以跑通多条WS链接，成功解决了我的问题。

### 使用
将paho-mqtt.js下载下来放入自己的工程文件中，API和[paho.mqtt.wxapp](https://github.com/tennessine/paho.mqtt.wxapp)的里面的完全一样（即和paho.mqtt.js相同）。

### 联系
E-mail: vkbo@qq.com