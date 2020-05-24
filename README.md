# zS7
**斐讯S7体脂称个人固件.**

S7体脂称因为服务器关闭,无法使用.(不过好像有其他app使用,所以并不是一定要刷机)

为此,开发供自己使用的FW及对应app,确保自己能够正常使用此设备.取名为zS7.

注意**当前不支持体脂,只支持体重功能**.后期也不一定会支持体脂.请知悉



建立了个QQ群,有问题可以加入来讨论:**459996006**  [点这里直接加群](//shang.qq.com/wpa/qunwpa?idkey=9104eabd6131d856b527ad89636fc603eb745a5d047e8b45d183165c8e607e59)  (收费群,请用android或pc入群. 支持我请加群或通过app端打赏我)(如果提示禁止入群,可能为付费群的一些问题,可以晚点再试)

也可以发送邮件给我:zip_zhang@foxmail.com  (邮件较多,可能会较晚回复)



> ### 作者声明
>
> 注意: 本项目主要目的为作者本人自己学习及使用S7而开发,仅个人开发,可能无法做到完整的测试,所以不承担他人使用本项目照成的所有后果.
>
> 暂时不开源,不需要激活码刷机即可使用.
>
> **严禁他人将本项目用户用于任何商业活动.个人在非盈利情况下可以自己使用,严禁收费代刷等任何盈利服务.**
>
> 有需要请联系作者:zip_zhang@foxmail.com



## 特性

本固件使用斐讯S7体脂称硬件为基础,实现以下功能:

- [x] 体重测量(体重数据为原厂获取,精度和原厂无区别)

- [x] 固件内记录10组体重记录

- [x] 原厂加热功能,(必须接电源)

- [x] ota在线升级

- [x] MQTT服务器连接控制

- [x] 无服务器时使用UDP通信

- [ ] 通过mqtt连入homeassistant(配置文件还没完成)

  

  

## 前言(必看)

- 除非写明了`如果你不是开发人员,请忽略此项`之类的字眼,否则,请**一个字一个字看清楚看完**整后再考虑动手及提问!很可能一句话就是你成功与否的关键!

- 烧录固件需要烧录器:ttl串口烧录器即可,一般刷机的人应该都有,淘宝价格大概为2-5元

- 使用此固件,需要app端配合,见[SmartControl_Android_MQTT](https://github.com/a2633063/SmartControl_Android_MQTT).

- app只有android,因ios限制,本人不考虑免费做ios开发.(不要再问是否有ios端).

- 本文文档还在编写更新中,部分文档还未完成.

  

> 虽然没有ios端,但固件支持homeassistant,可以使用安卓APP配置完成后,连入homeassistant后,使用ios控制. APP主要仅为第一次使用配对网络及配置mqtt服务器时使用,之后可以用homeassistant控制不再使用app.

> 如果你不知道什么是mqtt或homeassistant,所有有关的内容可以跳过.

> 如果你有任何问题,可以直接在此项目中提交issue,或给我发送邮件:zip_zhang@foxmail.com,邮件标题中请注明[zS7].
>



## 开始

整体流程如下:拆开S7,将固件/烧录器/pc互相连接,在pc运行烧录软件进行烧录,烧录固件.

烧录完成后,首次使用前配对网络并配置mqtt服务器,之后就可以使用了.



## 拆机接线及烧录固件相关

见[固件烧录](https://github.com/a2633063/zS7/wiki/固件烧录)

烧录固件完成后,即可开始使用



## 开始使用/使用方法

见[开始使用](https://github.com/a2633063/zS7/wiki/开始使用)



## 接入home assistant

见[homeassistant接入](https://github.com/a2633063/zS7/wiki/homeassistant接入)



## 其他内容



### 通信协议

> 此项为专业开发人员准备,如果你不是开发人员,请跳过此项

本项目为防止被低素质人员在我不知情的情况下拿去商用,所以本项目暂时不考虑开源,为了其他开发人员开发自己的控制软件,将通信协议开放

所有通信协议开源,你可以自己开发控制app或ios端

见[通信协议](https://github.com/a2633063/zS7/wiki/通信协议)



### FAQ

见 [FAQ](https://github.com/a2633063/SmartControl_Android_MQTT/wiki/FAQ)



### 文档更新日志

无

