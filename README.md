# 超详细的V免签支付系统搭建图文教程
## V免签(PHP) 是基于Thinkphp5.1 + mysql 实现的一套免签支付程序，主要包含以下特色：

1.收款即时到账，无需进入第三方账户，收款更安全

2.提供示例代码简单接入

3.超简单Api使用，提供统一Api实现收款回调

4.免费、开源，无后门风险

5.支持监听店员收款信息，可使用支付宝微信小号/模拟器挂机，方便IOS用户

6.免root，免xp框架，不修改支付宝/微信客户端，防封更安全

**V免签现已开发了免费PC监控端：** https://gitee.com/pmhw/Vpay

**v免签官方源码：** https://github.com/szvone/vmqphp   

**v免签安卓监控端：** https://github.com/szvone/VmqApk

```diff
+ this will be highlighted in green
- this will be highlighted in red
```

- ![#f03c15](https://placehold.it/15/f03c15/000000?text=+) `#f03c15`
- ![#c5f015](https://placehold.it/15/c5f015/000000?text=+) `#c5f015`
- ![#1589F0](https://placehold.it/15/1589F0/000000?text=+) `#1589F0`

### <table><tr><td bgcolor=#FF83FA>演示环境基于宝塔面板搭建，使用nginx1.18、php7.3、mysql5.6 已实测该环境正常搭建可用</td></tr></table>

### 该程序不支持<font color=red>PHP7.4</font>，请使用$\color{#FF0000}{PHP5.6以上~7.3}$  请严格按照教程步骤来搭建，搭建后首页登录就是后台，不需要访问域名/admin！默认账密均为admin

1、下载v免签压缩包，上传至服务器并解压

2、关闭防跨站攻击，设置运行目录为public并保存

![输入图片说明](https://img.a17cn.admin17.net/wp-content/uploads/2022/04/202107252154189798629.png "屏幕截图.png")

3、设置伪静态为thinkphp并保存

![输入图片说明](https://img.a17cn.admin17.net/wp-content/uploads/2022/04/202102041914496344816.png "屏幕截图.png")

4、设置默认文档，将index.html放在第一行并保存（这里改完顺序点击添加就是保存）

![输入图片说明](https://img.a17cn.admin17.net/wp-content/uploads/2022/04/202105211447241793965.png "屏幕截图.png")

5、打开网站路径/config/database.php ，设置好你的mysql账号密码并保存

![输入图片说明](https://img.a17cn.admin17.net/wp-content/uploads/2022/04/202105211511401546612.png "屏幕截图.png")

6、导入数据库文件vmq.sql到服务器里

![输入图片说明](https://img.a17cn.admin17.net/wp-content/uploads/2022/04/202105211438021034460.png "屏幕截图.png")

7、至此网站搭建完毕，请访问后自行修改配置信息！默认后台账号和密码均为admin

前台演示图

![输入图片说明](https://img.a17cn.admin17.net/wp-content/uploads/2022/04/202105211522596612129.png "屏幕截图.png")

后台演示图

![输入图片说明](https://img.a17cn.admin17.net/wp-content/uploads/2022/04/202105211531351044473.png "屏幕截图.png")
![输入图片说明](https://img.a17cn.admin17.net/wp-content/uploads/2022/04/202105211532017407056.png "屏幕截图.png")


v免签原理为监控收款后手机的通知栏推送消息，所以请保持微信/支付宝/v免签监控端后台正常运行，且添加到内存清理白名单，防止后台被杀！
v免签面向用户是个人开发者，如果你不懂如何搭建网站，那么v免签不适合你的使用！
v免签的原理是监控手机收到收款后的通知栏推送信息，所以不适合于商用多用户的情况，如果你想用于商用，需自行二次开发！
v免签是免费开源产品，所有程序均开放源代码，是不收费的，v免签使用具有一定的技术门槛，请自行研究！
v免签的监控端并不适配所有手机，遇到手机无法正常使用的时候，请您更换手机或使用模拟器挂机！


|||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||


# V免签-PC监控端更新界面
![输入图片说明](https://images.gitee.com/uploads/images/2021/0529/131037_d2560369_4920524.png "屏幕截图.png")

![输入图片说明](https://images.gitee.com/uploads/images/2021/0529/131046_1ba7f447_4920524.png "屏幕截图.png")

![输入图片说明](https://images.gitee.com/uploads/images/2021/0529/131054_fbe62667_4920524.png "屏幕截图.png")

#### 介绍
V免签pc监控端更新界面
支持微信、支付宝双端监听

#### 使用说明

1.  下载软件
2.  配置域名、密钥

#### 版本更新

持续更新中~~~ 点击顶部star 点亮小星星是对我最大的支持 

问题反馈：
qq群455123230（已满）
qq群757149396

市面上有很多圈狗，打着开源的旗号收费大多都是二改圈钱，其中包含二改V免签以及多用户V免签等等（只要会简单编程都可以做），没有任何技术可言，本人开发的（多用户免签）捷支付后续也会开源，10年开发经验重塑底层逻辑，app无障碍监听，pc稳定监听（以及2021最新方法，无视风控全网首发，），所以真正有实力技术有人品的是不会圈钱的，请大家擦亮眼镜！

作者声明:很多找我加功能的，我有自己的进度，首先我也不差这点钱其次也有自己的事要做如果付费可以加班帮你提前做，不然请耐心等待，那些没有必要的功能是不会加，因为此程序主要针对V免签，不收任何费用完全利用空余时间开放的，如果你想自己做免签适配自己的平台请联系我定制！ qq32579135 技术过硬 :cow: 。


最新更新地址：[https://pmhapp.com/](https://pmhapp.com/)

++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++

更新地址更换为 [https://pmhapp.com/](https://pmhapp.com/)


**Vpay监控 5.3 稳定版** [https://wwi.lanzoui.com/iLVxxtdud9e](https://wwi.lanzoui.com/iLVxxtdud9e)

更新日志

1.更新dll（支持当前最新版微信 3.3.5.50）

2.增加店员收款 监听店长昵称



**Vpay监控 5.2 稳定版** [https://wwi.lanzoui.com/ifw8zt4ngli](https://wwi.lanzoui.com/ifw8zt4ngli)

更新日志

1.修复微信店员监听验签失败问题

2.声明微信官网下载的微信和本地升级的微信版本号不一致，（默认手动升级的版本号为最新）可以打包本地的微信到服务器使用



 **Vpay监控 5.1 稳定版** [https://wwi.lanzoui.com/iAXgpsazbpe](https://wwi.lanzoui.com/iAXgpsazbpe)

更新日志

1.更新最新微信版本Hook 3.3.5.34

2.修复支付宝程序_延时问题



 **Vpay监控 5.O** 过渡版本




 **Vpay监控 4.9 稳定版**  [https://wwi.lanzoui.com/iLZ9dro5oyj](https://wwi.lanzoui.com/iLZ9dro5oyj)

更新日志

1.增加邮箱通知（收款、程序异常、订单异常等等）

2.修复使用文档打开异常

3.增加智能物联（预计下个版本开放，q群指令管理）




 **Vpay监控 4.8 稳定版**  [https://wwi.lanzoui.com/i5b4zrkkamj](https://wwi.lanzoui.com/i5b4zrkkamj)

更新日志

紧急修复接口。



 **Vpay监控 4.7 稳定版**  [https://wwi.lanzoui.com/iXxHrrk4g7e](https://wwi.lanzoui.com/iXxHrrk4g7e)

更新日志

1.彻底解决支付宝10分钟回调问题

2.解决支付宝0元订单推送

3.调整支付宝订单刷新到顶部



 **Vpay监控 4.6**  [https://wwi.lanzoui.com/iteaqrhk57g](https://wwi.lanzoui.com/iteaqrhk57g)


更新日志

1.增加设置代理IP功能（适配国外vps环境）

2.增加支付宝接口通道选择

3.解决支付宝掉单问题

4.优化多线程处理机制



 **Vpay监控 4.5**  [https://wwi.lanzoui.com/ixqzCr3vl0h](https://wwi.lanzoui.com/ixqzCr3vl0h)

更新日志：

增加微信商家版店员监听消息处理



 **Vpay监控 4.4**  [https://wwi.lanzoui.com/is1KXr1vm4f](https://wwi.lanzoui.com/is1KXr1vm4f)

更新日志：

1.更改支付宝循环方法

2.增加微信店员监控消息处理

3.支持当前最新版本微信 3.3.0.115



 **Vpay监控 4.3**  [https://wwi.lanzoui.com/iKHXuqr9tab](https://wwi.lanzoui.com/iKHXuqr9tab)

更新日志：

1.修复支付宝已知问题

2.增加刷新频率

3.更新获取订单机制



 **Vpay监控 4.2**  [https://wwi.lanzoui.com/ic8T7qpb4fg](https://wwi.lanzoui.com/ic8T7qpb4fg)

更新日志：

1.增加启动心跳音效

2.更新Hook支持微信版本 3.3.0.104 

3.修复必须要关注微信收款助手问题

4.增加新手使用文档



 **Vpay监控 4.1**  [https://wwi.lanzoui.com/i4p3lqnm1bi](https://wwi.lanzoui.com/i4p3lqnm1bi)

紧急修复



 **Vpay监控 4.0**  [https://wwi.lanzoui.com/i6loUqn4kcf](https://wwi.lanzoui.com/i6loUqn4kcf)

更新日志：

1.优化目前已知问题

2.解决支付宝阿里旺旺掉单现象

3.移除支付宝不稳定版，修改ie代理问题

4.支持微信版本号 3.3.0.93



 **Vpay监控 3.9**  [https://wwi.lanzoui.com/iYv1Yql4n1a](https://wwi.lanzoui.com/iYv1Yql4n1a)

更新HOOK不改版本号，自行选择
支持微信版本号 3.3.0.93



 **Vpay监控 3.9**  [https://wwi.lanzoui.com/iYsDQql2kcb](https://wwi.lanzoui.com/iYsDQql2kcb)

更新日志：
优化支付宝监听
增加阿里旺旺监听（测试阶段）
修改微信hook地址
支持微信版本号 3.3.0.84



 **Vpay监控 3.8**  [https://wwi.lanzoui.com/i68mvprsz0f](https://wwi.lanzoui.com/i68mvprsz0f)

更新日志：

适配最新版微信Hook，优化退出WechatBrowser.exe



**Vpay监控 3.7**  [https://wwi.lanzoui.com/iLUEtpq4q4f](https://wwi.lanzoui.com/iLUEtpq4q4f)

哈勃分析：[点此进入](https://habo.qq.com/file/showdetail?pk=ADcGYF1sB2QIMFs9U2s%3D)

更新日志：

更新支付宝监听，防风控更稳定；

修改获取订单显示位置，顶部显示。



 **Vpay监控 3.6**  [https://wwi.lanzoui.com/iqxvHpo0o2f](https://wwi.lanzoui.com/iqxvHpo0o2f
)

更新日志：

修复端口被占用，导致无法继续创建端口获取消息问题。



 **Vpay监控 3.5**  [https://wwi.lanzoui.com/iJK0upnyusf](https://wwi.lanzoui.com/iJK0upnyusf)

更新日志：

修复启动初始化端口，解决长时间微信会断线。



 **Vpay监控 3.4**  [https://wwi.lanzoui.com/igLvzpmt41g](https://wwi.lanzoui.com/igLvzpmt41g)

更新日志：

1.修复支付宝登录显示

2.修复部分微信用户没有订阅收款助手无法回调



 **Vpay监控 3.3**  [https://wwi.lanzoui.com/igLvzpmt41g](https://wwi.lanzoui.com/igLvzpmt41g)

更新日志：

紧急修复微信Hook偏移


**Vpay监控 3.2**  [https://wwi.lanzoui.com/iDgUJplkyje](https://wwi.lanzoui.com/iDgUJplkyje
)

更新日志：
1.增加收款后播报语音功能
2.优化了fd劫持ie
3.增加了右下角版本号显示


 **Vpay监控 3.1**   [https://wwi.lanzoui.com/i654Rpkb0bc](https://wwi.lanzoui.com/i654Rpkb0bc
)

更新日志：
1.增加了微信监听
2.优华心跳频率
