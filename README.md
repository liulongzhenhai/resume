### 个人信息
![enter image description here](https://raw.githubusercontent.com/liulongzhenhai/markdownphoto/master/my.jpg)
 - 刘龙振海 / 男 / 1988.7
 - 本科 / 武汉理工大学 / 计算机软件 
 - 工作年限：8年
 - 联系方式：18688185397 / [liulongeric@gmail.com](mailto:liulongeric@gmail.com)
 - 期望职位：Android高级程序员
 
----------

  
### 技能清单
- Java / c# / VB / C / PHP 
- lambda / stream 
- RxJava(1.1 / 2.0) / RxAndroid(1.1 / 2.0)
- Git / SVN
- Retrofit / OkHttp / Glide / Butterknife / EventBus
- Arouter / BRVAH / Zxing

---

### 工作经历
-  一点智慧科技有限公司  `Android 高级工程师`（ 2017.8 ~至今 ）
	+ 45天、1人完成整个项目的重构，提高了流畅度，健壮性
	+ 上线单片机项目，搭建基本 Android 串口通信代码
	+ 上线2个项目，**一点智慧App**、**一点智慧会议室Pad**
	+ 共迭代1次大版本，10次小版本
	+ 重新整理Android 组的开发架构、开发规范、UI设计，分解项目Model，在后续的pad端验证了分解的合理和重用度
- 万门教育科技有限公司  `技术经理` （ 2016.6 ~2017.6）
	+ 负责技术团队的管理、需求分析、技术调研、客服、招聘
	+ 从CC视频平台过度到自主研发的视频平台上，每月为公司省4-5万，防止了视频泄露，我主要负责移动端的实施方案
	+ 完善了研发流程，提升迭代速度，尽量2-3星期一迭代，统计各数据，明显改善各平台的错误率；帮助客服更方便收集问题信息；提出视频交互的方案；视频加密方案三步走
	+ 从5人开始搭建技术团建（Android 4人、IOS 2人、WEB 3人、后台 2人、测试 2人、UI 2人、产品 1人、CTO 1人）
- 北京穷游天下科技有限公司 `Android 工程师`（2014.11~2016.6）
	+  负责《穷游锦囊APP》项目 Android开发和进度，完成了业务和框架改版，搭建Rx开发框架
	+  参与《穷游APP》项目Android 开发，完成“在路上”功能模块开发，完成了4.0大版本
	+  负责《JOY》的Android开发，负责个人信息模块、锦囊以及Android进度
	+  参与技术分享以及招聘工作
- 远光软件股份有限公司 `Android 工程师` （2011.7~2014.10）
	+  负责Android 的项目开发以及框架搭建，减少Adapter 60%的代码，减少网络请求缓存处理逻辑等
	+  负责Android 技术分享，定期分享讨论，组织和外部技术人员交流
- 广州掌景科技有限公司 `Android 工程师`  （2009.7~2011.7）
	+  参与《开心号簿》Windows Mobile 研发并主动把项目转移到Android上
	
-----
### 近期项目经验
- 一点智慧、一点智慧Pad `2名Android`
	+ 主要负责：```开发框架```、```QR Code扫描```、```蓝牙开锁```、```会议室/工位预定```、```订单```
	+  主要功能：**工位/会议室预定**、**QR Code扫描**、**蓝牙开门**
	+  使用RxJava2+Retrofit2+OkHttp3 做网络请求，配合自定义的Annotation对接口进行缓存策略定义，md5 url作为文件名保存在本地，文件以Disk Lru形式保存，主要从原来的Rx1.1转到2.0的代码上修改
	+  初步使用Lambda和Java8 特性在项目中，减少代码量，优化阅读，使用第三方Stream库做兼容
	+  改善蓝牙搜索，结合BLE和广播形式，对搜索结果进行整合
	+  项目采用模块化，使用**org.greenrobot.eventbus 3 **进行数据回调
	+  使用OTG 串口通讯协议对RS232单片机联动，单片机连接电磁铁门，实现Pad应用在业务完整下进行开锁和关门操作
	+  使用netty 包进行socket通讯，
	+  简单的icon使用svg格式，在适配上更加灵活，减少包大小
	+  使用butterknife、arouter、zxing、glide4.0、BRVAH、Realm等第三方库
	+  封装微信支付，阿里支付sdk；Builder模式封装分享sdk
	
- 万门大学、万门中学、万门Tv `4名Android`
	+ 主要负责：```下载```、```视频```、```开发框架```
	+  主要功能： **视频播放/下载**、**直播/IM功能**、**课程购买**
	+  视频采用m3u8，下载视频使用AsyncTask单线程对视频进行下载，采用LocalBroadcastReceiver进行广播
	+  参考Google MVP 架构模式搭建框架，为项目添加findebugs、checkstyle配置进行项目走查，为了更好了解对方的代码，提升代码质量，从代码中提前发现问题，采用提pr形式进行代码review 合并
	+  部分页面转为H5页面，利用JS、链接跳转进行native交互
	+  拆解项目为多个Model，在不同的项目，建立res Model作为样式的差异化
- 穷游 穷游锦囊 `12名Android`
	+  主要负责：```个人信息相关```、```在路上```、```锦囊```、```酒店```、```分享整合```
	+  主要功能： **折扣**、**当地游**、**锦囊**、**社区**
	+  使用RxJava1.1+Retrofit+OkHttp ，为防止用户间的缓存错乱，使用Annotation加入Tag标识，提供五种请求方法，只读网络，串行/并行读取缓存和网络，只读缓存，有缓存使用缓存无则网络，使用rxlifecycle进行Rx生命周期管理
	+  使用WebView展示锦囊信息，种cookie，完成webview的各项本地操作，如电话、查看图片、activity内跳转等
	+  通过build 的productFlavors 建立测试和开发环境以及一些配置信息，避免打包导致的错误
	+  使用RecyclerView多布局编写日历选择控件，并显示节假日信息
	+   统一处理共同的业务，如网络请求的业务处理引发的UI操作和错误提示
- 民政通 `6名Android`
	+ 主要负责：```二维码```、```开发框架```、```短信猫```
	+ 主要功能： **咨询信息**、**办证**、**二维码证件**
	+ 封装ListView Adapter，使用Map保存控件，减少ViewHolder和findViewById的代码
	+  封装网络请求工具类 HttpConnection+AsyncTask+fastjson，使用文件缓存形式缓存数据
	+  自封装ImageLoader ，使用LRU 实现二级缓存，内存缓存中需要的Size图片，本地文件缓存原始图片
	+ 通过ADB Socket到手机，实现手机收发彩信，编写PC客户端，Socket到服务器，采用大端法形式进行拆包 
	+ 针对cmwap和cmnet、wifi下对socket链接的处理，编写心跳包维持链接，采用大端法进行数据解包，采用NIO技术，逐段解析包
