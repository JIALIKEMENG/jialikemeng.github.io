一. 下载并安装ADB软件驱动
1. 下载：
[官网](https://developer.android.com/studio/releases/platform-tools.html)需要快乐上网，已转存[蓝奏云](https://yooofox.lanzouoo.com/i13yuhc8v2f)。
2. 安装：
解压ADB工具的压缩包至某目录下，在桌面右键我的电脑→属性→高级系统设置→高级→环境变量→在系统变量中选择Path→点击编辑→点击新建，输入ADB工具所在路径（即*:\****\****\****\platform-tools）→点击确定→点击确定→点击确定。
二、打开手机USB调试模式
打开设置→我的设备→全部参数→点击MIUI版本10次，进入开发者模式，返回设置→更多设置→开发者选项→USB调试→等待5秒后点击允许。
三、卸载应用
1、调试：
使用win+r键打开运行窗口，输入cmd打开命令提示符，在命令提示符窗口中输入adb，当看到有如图所示就说明环境配置成功；输入adb devices命令，如果设备已正确连接，你将看到设备列表，其中会显示设备的序列号或名称；如果没有设备显示，或者显示“no devices/emulators found”，则说明设备未被正确识别；显示"List of devices attached"意味着ADB（Android Debug Bridge）没有检测到任何连接的Android设备或模拟器，需要检查USB连接、是否启用了USB调试模式等。
2、卸载：
输入卸载命令，回车，如果出现“Success”表示删除成功。
adb shell pm uninstall --user 0 com.miui.systemAdSolution（小米系统广告解决方案，必删）
adb shell pm uninstall --user 0 com.miui.analytics（小米广告分析，必删）
adb shell pm uninstall --user 0 com.xiaomi.gamecenter.sdk.service  （小米游戏中心服务）
adb shell pm uninstall --user 0 com.xiaomi.gamecenter  （小米游戏中心）
adb shell pm uninstall --user 0 com.sohu.inputmethod.sogou.xiaomi  （搜狗输入法）
adb shell pm uninstall --user 0 com.miui.player  （小米音乐）
adb shell pm uninstall --user 0 com.miui.video  （小米视频）
adb shell pm uninstall --user 0 com.miui.notes  （小米便签）
adb shell pm uninstall --user 0 com.miui.translation.youdao  （有道翻译）
adb shell pm uninstall --user 0 com.miui.translation.kingsoft  （金山翻译）
adb shell pm uninstall --user 0 com.android.email  （邮件）
adb shell pm uninstall --user 0 com.xiaomi.scanner  （小米扫描）
adb shell pm uninstall --user 0 com.miui.hybrid  （混合器）
adb shell pm uninstall --user 0 com.miui.bugreport  （bug 反馈）
adb shell pm uninstall --user 0 com.milink.service  （米连服务）
adb shell pm uninstall --user 0 com.android.browser  （浏览器）
adb shell pm uninstall --user 0 com.miui.gallery  （相册）
adb shell pm uninstall --user 0 com.miui.yellowpage  （黄页）
adb shell pm uninstall --user 0 com.xiaomi.midrop  （小米快传）
adb shell pm uninstall --user 0 com.miui.virtualsim  （小米虚拟器）
adb shell pm uninstall --user 0 com.xiaomi.payment  （小米支付）
adb shell pm uninstall --user 0 com.mipay.wallet  （小米钱包）
adb shell pm uninstall --user 0 com.android.soundrecorder  （录音机）
adb shell pm uninstall --user 0 com.miui.screenrecorder  （屏幕录制）
adb shell pm uninstall --user 0 com.android.wallpaper  （壁纸）
adb shell pm uninstall --user 0 com.miui.voiceassist  （语音助手）
adb shell pm uninstall --user 0 com.miui.fm  （收音机）
adb shell pm uninstall --user 0 com.miui.touchassistant  （悬浮球）
adb shell pm uninstall --user 0 com.android.cellbroadcastreceiver  （小米广播）
adb shell pm uninstall --user 0 com.xiaomi.mitunes  （小米助手）
adb shell pm uninstall --user 0 com.xiaomi.pass  （小米卡包）
adb shell pm uninstall --user 0 com.android.thememanager  （个性主题管理）
adb shell pm uninstall --user 0 com.android.wallpaper  （动态壁纸）
adb shell pm uninstall --user 0 com.android.wallpaper.livepicker  （动态壁纸获取）
adb shell pm uninstall --user0 com.baidu.input_mi（百度输入法）
adb shell pm uninstall --user 0 com.xiaomi.smarthome（米家）
adb shell pm uninstall --user 0 com.miui.virtualsim（全球上网）
adb shell pm uninstall--user 0 com.mi.liveassistant（小米直播助手）
adb shell pm uninstall --user 0 com.miui.hybrid（快应用）
adb shell pm uninstall --user 0 com.xiaomi.market  （应用商店）
adb shell pm uninstall --user 0 com.android.quicksearchbox  （自带搜索）
adb shell pm uninstall --user 0 com.miui.voiceassist  （小爱同学）
adb shell pm uninstall --user 0 com.xiaomi.mibrain.speech  （小爱语音引擎）

MIUI 12.5含EU版内置APP：

package:com.miui.contentextension（传送门）
package:com.bsp.catchlog（CatchLog反馈bug时收集日志）
package:com.xiaomi.gamecenter.sdk.service（游戏服务）
package:com.android.mms.service（彩信服务）
package:com.android.browser（浏览器）
package:com.miui.daemon（Miu[IDA](https://www.52pojie.cn/thread-1874203-1-1.html)emon用户信息收集）
package:com.miui.player（音乐）
package:com.miui.miservice（服务与反馈）
package:com.miui.vpnsdkmanager（游戏网络加速）
package:com.miui.bugreport（用户反馈）
package:com.android.cellbroadcastreceiver（小区广播）
package:com.miui.mishare.connectivity（小米互传）
package:com.miui.newhome（内容中心）
package:com.miui.video（小米视频）
package:com.sohu.inputmethod.sogou.xiaomi（搜狗输入法）
package:com.miui.touchassistant（悬浮球）
package:com.xiaomi.gamecenter（游戏中心）
package:com.miui.yellowpage（生活黄页）
package:com.miui.accessibility（小米闻声）
package:com.miui.voiceassist（小爱同学）
package:com.miui.fmservice（收音机调频服务）
package:com.miui.newmidrive（小米云盘）
package:com.miui.screenrecorder（屏幕录制）
package:com.xiaomi.miplay_client（投屏）
package:com.miui.fm（收音机）
package:com.android.providers.calendar（日历存储）
package:com.xiaomi.account（小米账户）
package:com.xiaomi.mi_connect_service（小米互联通信服务）
package:com.xiaomi.micloud.sdk（小米云服务）
package:com.android.htmlviewer（HTML查看器）
package:com.miui.gallery（相册）
package:com.android.quicksearchbox（搜索）
package:com.xiaomi.payment（米币支付）
package:com.android.soundrecorder（录音机）
package:com.google.ar.lens（智能镜头）
package:com.miui.backup（备份）
package:com.miui.micloudsync（MiCloudSync）
package:com.miui.daemon（MiuiDaemon）
package:com.miui.huanji（小米换机）
package:com.mi.health（健康）
package:cn.wps.moffice_eng.xiaomi.lite（WPS）
package:com.mfashiongallery.emag（锁屏画报）
package:com.android.calendar（日历）
package:com.miui.compass（指南针）
package:com.miui.aod（万象息屏）
package:com.miui.cit（CIT手机测试）
package:com.android.printspooler（打印处理服务）
package:com.miui.personalassistant（智能助理）
package:com.miui.misound（耳机音效）
package:com.android.bips（系统打印服务）
package:com.android.fileexplorer（文件管理）
package:com.google.android.apps.cloudprint（云打印）
package:com.miui.cloudbackup（桌面云备份）
package:com.android.cellbroadcastreceiver（小区广播）
package:com.xiaomi.xmsf（小米服务框架）
package:com.google.android.tts（google文字转语音引擎）
package:com.android.calllogbackup（通话记录备份）
package:com.miui.freeform（自由窗口）
package:com.miui.miwallpaper.mars（火星超级壁纸）
package:com.xiaomi.joyose（运动计步）
package:com.miui.nextpay（小米支付）
package:com.miui.notes（便签）
package:com.google.android.feedback（应用商店反馈代{过}{滤}理程序）
package:com.google.android.syncadapters.calendar（google日历同步）
package:com.miui.cloudservice（小米云服务）
package:com.miui.touchassistant（悬浮球）
package:com.miui.miwallpaper.earth（地球超级壁纸）
package:com.miui.calculator（计算器）
package:com.android.wallpaper.livepicker（动态壁纸获取）
package:com.miui.miwallpaper（壁纸）
package:com.miui.miwallpaper.geometry（几何超级壁纸）
package:com.android.bookmarkprovider（Bookmark Provider）
package:com.miui.weather2（天气）
package:com.xiaomi.scanner（扫一扫）
package:com.android.email（邮件）
package:com.android.providers.userdictionary（用户字典）
package:com.google.android.gms.location.history（google位置记录）
package:com.android.location.fused（一体化位置信息）
package:com.android.deskclock（时钟）
package:com.android.thememanager（主题壁纸）
package:com.xiaomi.bsp.gps.nps（卫星定位）
package:com.android.traceur（系统跟踪）

 MIUI 国际版（欧版 miui.eu）应用包名（欧版可以随便删）：
com.google.android.googlequicksearchbox （Google）
com.miui.miservice （服务与反馈）
com.mi.health （健康）
com.mi.globalbrowser （国际版浏览器）
com.miui.huanji （小米换机）
com.miui.newmidrive （小米云盘）
com.miui.bugreport （用户反馈）
com.miui.personalassistant （智能助理）
com.android.hotwordenrollment.xgoogle （谷歌助理1）
com.android.hotwordenrollment.okgoogle （谷歌助理2）
com.xiaomi.mirecycle （小米回收）
com.miui.videoplayer （小米视频国际版）
com.google.android.projection.gearhead （Google Auto/Google 汽车）
com.google.android.gms.location.history （Google 地理位置历史记录）
com.google.ar.lens （Google 智能（虚拟）摄像头）

参看：
[分享自用小米手机ADB命令删除系统内置应用](https://www.mydigit.cn/forum.php?mod=viewthread&tid=54419)
[使用ADB免ROOT免解锁卸载Android系统内置App 附MIUI12.5内置包名](https://www.52pojie.cn/thread-1416346-1-1.html)
[使用ADB不root删除小米MIUI系统自带应用](https://dt27.cn/android/use-adb-to-delete-the-builtin-application-of-miui/)
[adb删除卸载小米、红米手机(K50)预装系统软件和系统服务](https://zhuanlan.zhihu.com/p/632050682)
[MIUI 12.5 预装应用/服务停用/卸载](https://zhuanlan.zhihu.com/p/474778718)
