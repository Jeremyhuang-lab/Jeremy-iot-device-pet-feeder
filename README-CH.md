# Jeremy-iot-device-pet-feeder
该项目是使用Tuya SDK开发的，该项目使您能够快速开发连接和控制许多设备的智能方案的品牌应用程序。
有关更多信息，请访问Tuya开发人员网站。


1.产品名称
==
智能宠物喂食器

2.产品创建原因
==

衣服是为了抵御寒冷，然后才被赋予更多内涵。
火是为了取暖和阻吓野兽，然后才被用于能源。
工具是为了更好获得产品，然后才进化为机器。
人类文明的进化不是懒惰，是人类一直在追求自己的舒适。

随着人们日益增长的物质生活需求和对美好生活的向往，目前许多各行各业，各个年龄阶层的人都开始养起来宠物，
但是当代打工人平时工作007，实在没有时间照顾小宠物，而且经过去年疫情事件，许多人因封城居家隔离，
不能前往工作地喂养宠物，因此，智能宠物喂食器应运而生。

3.产品功能
==
APP 控制  定时定量 自动出粮 科学的喂养计划 缺粮提醒 智能喂水  无水检测 环境监测语音控制 实时视频监控(待开发) 

APP控制通过涂鸦智能APP与涂鸦WIFI模组配合，移植相关SDK，使用官方调试助手测试功能

定时定量 通过单片机定时器定时每隔6小时使能电机转动，打开排粮口，持续2秒钟时间，2秒钟后，电机反转，排粮口关闭。

自动出粮，APP设置时间，发送指令控制单片机在相应时间出粮。

科学的喂养计划，客户长时间外出时，设置智能喂养模式，程序自动设置喂养计划，定时投放。

智能喂水，可以设置模具为一个排粮口，一个排水口，通过两个电机分别控制，打开相应舱门投放。

无水检测 可以通过干簧管或者铁片检水，原理是通过检测铁片在有水或者缺水状态时，电压的变化，用单片机ADC检测。

环境监测 加入一个温湿度传感器，当温度过高时，立即打开排水口，给宠物饮水，及改变相应喂养计划。

语音控制，通过涂鸦WIFI模组对接小度等智能语音，语音喂养。


实时视频监控，预计可以通过OPENCV或者是否可以通过涂鸦WIFI模组与其他视频设备连接，通过它们发送宠物实时视频。


4.部分设计细则
==
单片机主控选择国产8051单片机STC15W58S4或者选择STM32F103系列
电机驱动采用H桥驱动 单片机PWM控制有刷直流电机转速或者选择ULN2003驱动单极性步进电机同样用单片机PWM控制方向转速。

温湿度芯片可以选择SHT30或者DHT11

同时可以加入RGB灯光效果

可以的话利用3.3V升压5V芯片驱动UVC灯，定时给粮食饮用水消毒。

5.开发计划
==
1）3月15前准备物料
2）3月15-3月25日嵌入式开发、云开发
3）3月30日前整体调试。
