### ----2020.7.13（庚子年五月廿三）Monday -----

** 预防github打不开的B方案
可以设置推送同时推送到github和gitee
https://www.yuque.com/greyzeng/uzfhep/ycoqn4
这样就不怕github经常打不开了


【最新】解决Github网页上图片显示失败的问题
https://blog.csdn.net/qq_38232598/article/details/91346392


腾讯云轻量 24块钱，买个反代 gayhub 和 谷歌就好了
买个 国外服务器，安装nginx 设置反向代理 x 网站

***
Mr.Simple的专栏
https://blog.csdn.net/bboyfeiyu

kymjs张涛
https://blog.kymjs.com/

***
垂直方向的支持
ViewPager2可以在垂直方向上翻页，仅需要在布局文件添加一行代码

***
可怕！从简洁高效的角度来说，Kotlin比Java强太多了吧！难道Java真的要被替代了？
https://blog.csdn.net/colinandroid/article/details/80490040
Tip1- 更简洁的字符串
Tip2- 更好调用的函数：显式参数名/默认参数值
Tip3- 利用局部函数抽取重复代码
Tip4- 使用数据类来快速实现model类
Tip5- 用类委托来快速实现代理模式
Tip6- apply函数来简化代码
Tip7- 用函数型变量来简化回调
Tip9- let语句简化可空对象访问


***
Qt、WPF
UWP即Windows 10中的Universal Windows Platform

CEF （Chromium嵌入式框架）
DirectUI 界面库 DuiLib


### ----2020.7.12（庚子年五月廿二）Sunday -----
onTouch和onClick事件冲突（leo老师主讲-未看完）


### ----2020.7.11（庚子年五月廿一）Saturday -----
架构演进
一体架构
MVC：model独立出来，View是可以直接访问Model的
MVP：与MVC相比，与Model交互的部分由Presenter处理
MVVM：与MVP相比减少各种接口回调

MVC （Model-View-Controller)
MVP （Model-View-Presenter）
MVVM（Model-View-ViewModel）

MVC、MVP、MVVM模式的概念与区别
https://www.jianshu.com/p/ff6de219f988


### ----2020.7.10（庚子年五月二十）Friday -----

** 非技术问题

老师好，老师在多年开发经验里，如果拿到一个产品需求任务，如何能在开发初期及时发现里面风险点和坑点啊？
我是接到一个任务，不管三七二十一就排期开干，等到开发到半路才发现里面的坑，吃了好几次亏，现在想咨询老师有没有经验传授下哈
这个问题也不急，老师有时间整理整理，或者推荐相关资料也行

ZLL:
这种问题也不是三言两语说的清的

无:
就是工期能报长就报长，千万别觉得自己认为几天能搞完就一定能搞完。。多报几天总归没错。预留出自己如果遇到不会的问题，去解决问题的时间。

老梁:
工作量估算开发周期时间直接double  基本也就问题不大了

陈阳:
开发前先设计清楚工程框架

涂晓龙:
产品需求评审之后，加个技术评审的步骤，拆解需求，定技术方案，排期加冗余


JETT老师 ：
这个主要是思考两点
1.需要中有没有技术上做不到的
2.这个需求会不会在开发中变动
JETT老师：
还一个就是需求中是否会有没写明确，但技术上必需去做的，或是要主动去挖


正规项目组里是需要调研时间的，那些没做过的技术点需要先调研
调研完再排期，太复杂要让产品削减需求，或者排个长一点的工期


AV老师  16:54:51
这个其实也没有太多的想法，基本上就是排开了干
哈哈
AV老师  16:54:59
不过，要及时的去调整
多想到复用
类超过 400行代码一定要重构
另外，首先要选择一个app的架构：建议就是MVVM
然后，基于jetpack做开发
如果能用kotlin就用kotlin


https://github.com/liangjingkanji/Net   Android不是最强的网络请求

https://github.com/liangjingkanji/BRV   Android不是最强的列表库

***
androidx.cardview.widget.CardView
CardView实现阴影效果

***
VoIP
基于IP的语音传输（英语：Voice over Internet Protocol，缩写为VoIP）是一种语音通话技术，经由网际协议（IP）来达成语音通话与多媒体会议，也就是经由互联网来进行通信。
其他非正式的名称有IP电话（IP telephony）、互联网电话（Internet telephony）、宽带电话（broadband telephony）以及宽带电话服务（broadband phone service）。
VoIP可用于包括VoIP电话、智能手机、个人计算机在内的诸多互联网接入设备，通过蜂窝网络、Wi-Fi进行通话及发送短信。


### ----2020.7.9（庚子年五月十九）Thursday -----
CoordinatorLayout+Behavior实现嵌套滑动效果
Behavior只有是CoordinatorLayout的直接子View才有意义。可以为任何View添加一个Behavior。
Material Design里面的CoordinatorLayout是一个非常强大的控件，它接管了child组件之间的交互。
让你滑动交互使用更加方便简单，效果也更加强大，不需要像以前那样自己处理一坨什么乱七八槽的滑动,事件传递之类的处理了。
https://blog.csdn.net/jinfulin/article/details/77927719

***

foreach报java.util.ConcurrentModificationException异常问题解决：迭代器
1、将ArrayList改为CopyOnWriteArrayList在多线程环境中同样可以避免出现这个异常。
2、采用ConcurrentHashMap替换HashMap
3、采用同步锁等的方案

***
跨平台开发：Android和iOS平台上运行的应用

Cordova，PhoneGap 最优，毕竟十几年在哪，坑少，解决方案多。
React-Native, NativeScript 其次，要求些许英文的阅读能力(特别是 NativeScript)，这两种解决方案都可以尝试，但不建议作为首选项。
Flutter 和 Xarmarin，Xarmarin 我没用过，所以没有发言权。Flutter 不建议用于 production。

国内的Dcloud的Uniapp
app端就用echart，小程序端就用uchart

链接：https://www.zhihu.com/question/333817230/answer/903381349

***Android自定义动画
[Android自定义控件三部曲文章索引](https://blog.csdn.net/harvic880925/article/details/50995268)  

[自定义控件三部曲之动画篇(七)——ObjectAnimator基本使用](https://blog.csdn.net/harvic880925/article/details/50598322)  


motion动画详解
[ConstraintLayout 2.0新特性 MotionLayout制作炫酷动画](https://mp.weixin.qq.com/s/JkMJQLOUr3hoFf-eJ-OBDQ)  
[MontionLayout：打开动画新世界大门](https://mp.weixin.qq.com/s/Cs3_9vIC3IKrZ4KzBtKoYw)    


### ----2020.7.8（庚子年五月十八）Wednesday -----

https://www.jianshu.com/u/942d45d61f59
Android 消息处理机制（Looper、Handler、MessageQueue,Message）

周周大佬

https://www.jianshu.com/u/0d51dc41eff1



### ----2020.7.7（庚子年五月十七）Tuesday -----



插件化换肤


### ----2020.7.6（庚子年五月十六）Monday -----
Flywith24


[域名解析](https://www.ipaddress.com/)  

[如何利用 theme 与 style 更优雅地管理资源文件](https://github.com/Flywith24/Flywith24-Theme-demo)  

***
FlowLayout

[FlexboxLayout——实现灵活多变的瀑布流](https://www.jianshu.com/p/0723ff4123e1)  

[FlexboxLayout是什么?](https://www.jianshu.com/p/a8edc312fa3d)  
FlexboxLayout 可以理解为高级的 LinearLayout，因为这两个布局都将其子视图按序排列。
二者之间的重要差异在于 FlexboxLayout 具有 “换行” 的特性。
同时 FlexboxLayout 还为 RecycleView 提供了管理器 FlexboxLayoutManager。

***
[FlexboxLayout的使用说明书](https://zhuanlan.zhihu.com/p/29169416)  
google
https://github.com/google/flexbox-layout



### ----2020.7.5（庚子年五月十五）Sunday -----

论文整理



### ----2020.7.4（庚子年五月十四）Saturday -----
RxJava异步调用目前优于Kotlin协程

***
Jetpack Architecture Components
Lifecycle ViewModel LiveData Room
***
[synchronized的CPU原语级别是如何实现的？](https://www.cnblogs.com/ytxiao/p/12182679.html)  
**synchronized CPUY原语实现**
synchronized代码块主要是靠monitorenter和monitorexit这两个原语来实现同步的。

monitor的本质是依赖于底层操作系统的Mutex Lock实现，
操作系统实现线程间的切换需要从用户态到内核态的切换，切换成本非常高。


### ----2020.7.3（庚子年五月十三）Friday -----




胡志强
胡富国
耿彦波：当政所在地百姓口碑：大规模基建 
（X拆拆：季拆拆、仇拆拆） 

大同：昙曜和尚
云冈石窟皇帝

【陇上八州】
位於陇西地区的丝路要点
「沙洲」敦煌、「瓜州」安西、「肃州」酒泉、「甘州」张掖、
「凉州」武威、「兰州」兰州、「秦州」天水、「河州」临夏 等地，合称「陇上八州」

凉州：武威（雍州、姑臧、休屠，雍凉之都、天下要冲、梦幻之城）
甘州：张掖
肃州：酒泉
兰州：金城（皋、兰）
沙州：敦煌
瓜州：安西县
秦州：天水秦州区
河州：临夏
成州：成县

兰州，肃州，瓜州，沙州（敦煌），
甘州，凉州，渭州（陇西），成州（成县），秦州，
岷州（岷县），迭州（迭部），洮州（临潭），宁州（宁县），
庆州（庆阳），环州（环县），粟州和会州（会宁），文州（文县），阶州（武都）
武州（武都），南秦州（徽成），康州（康县，北周时期）

玉门关（甘肃省敦煌市城西北八十公里戈壁滩,一名小方盘城,是长城西端重要关口）
阳  关（甘肃省敦煌市西南七十公里古董滩）



### ----2020.7.2（庚子年五月十二）Thursday -----
MinGW(Minimalist GNU for Windows)   


### ----2020.7.1（庚子年五月十一）Wednesday -----

深入理解Kotlin协程----霍丙乾

Kotlin

**star projection(星投影）**

泛型约束 

```kotlin
fun <T : Comparable<T>> sort(list: List<T>) {
    // ……
}
```

***

Java 语言中，数组是协变的，泛型不是协变的

[Java泛型中的PECS原则](https://blog.csdn.net/xx326664162/article/details/52175283)

[What is PECS (Producer Extends Consumer Super)?](http://stackoverflow.com/questions/2723397/what-is-pecs-producer-extends-consumer-super/2723538#2723538)  

[深入理解 Java 泛型：类型擦除、通配符、运行时参数类型获取](https://blog.csdn.net/hustspy1990/article/details/78048493)  

PECS原则（控制读写）

java泛型：extends->读 |	super->写

Kotlin泛型：out->读  |	in->写



***

binder是Android通讯的血管

***
美团点评移动端基础日志组件 Logan

Xlog
elvishew -xLog
https://github.com/elvishew/xLog
Android logger, simple and pretty, powerful and flexible, all you need is here (updating)



***

Mars 是微信官方的跨平台跨业务的终端基础组件。

- comm：可以独立使用的公共库，包括 socket、线程、消息队列、协程等；
- xlog：高可靠性高性能的运行期日志组件；
- SDT： 网络诊断组件；
- STN： 信令分发网络模块，也是 Mars 最主要的部分。

***
[Java NIO Tutorial](http://tutorials.jenkov.com/java-nio/index.html)  
RandomAccessFile aFile     = new RandomAccessFile("data/nio-data.txt", "rw");
FileChannel      inChannel = aFile.getChannel();

***
buildTypes {//在android节点下
        release {
……
		debug{

***  Android多渠道打包 **
flavorDimensions
productFlavors
defaultConfig或buildType中配置Mainfestplacehoders：
android {
    compileSdkVersion 23
    buildToolsVersion '25.0.0'
    defaultConfig {
        manifestPlaceholders = [STAT_KEY    : "1111111111111",
                               		STAT_CHANNEL: "rrrrF"]
https://blog.csdn.net/f552126367/java/article/details/86502481  

[Android项目中gradle文件里面的productFlavors一些常用配置](https://www.jianshu.com/p/0ff4b5f5e892)  



---

[Gradle多渠道打包(动态设定App名称，应用图标，替换常量，更改包名，变更渠道)](https://www.jianshu.com/p/533240d222d3)  
不同环境，不同包名；
不同环境，修改不同的 string.xml 资源文件；
不同环境，修改指定的常量；
不同环境，修改 AndroidManifest.xml 里渠道变量；
不同环境，引用不同的 module。



***
zip文件格式EOCD(End of Central Directory record)
***

【JMeter】是Apache组织开发的基于Java的压力测试工具。
***

[文件类型魔数](https://www.jianshu.com/p/114340fec1b2)  

***
依赖库地址
maven { url 'http://maven.aliyun.com/nexus/content/groups/public/' }
maven { url 'https://jitpack.io' }
maven { url 'https://dl.bintray.com/umsdk/release' }
maven { url "http://mvn.mob.com/android" }

jcenter()
google()

***
https://www.cnblogs.com/chaojimali/p/12750936.html

enter passphrase for key '~/.ssh/id_rsa'
避免每次pull或者push都要输入密码

enter passphrase for key '~/.ssh/id_rsa'


1、输入下边命令；

ssh-keygen -p [-P old_passphrase] [-N new_passphrase] [-f keyfile]


2、实例：旧密码为123465

ssh-keygen -p -P "123456" -N '' -f ~/.ssh/id_rsa

***

开发技术栈(Android)
DB canvas OpenGL MVVM 音视频解码 socket http netty 串口通讯 rabbitmq


Android6.0(M)动态权限获取框架(github星)
Normal Permissions权限一般不涉及用户隐私，不需要用户进行授权，比如手机震动、访问网络等；
Dangerous Permission权限涉及到用户隐私的，需要用户进行授权，比如读取sdcard、访问通讯录等；

PermissionsDispatcher(10k)使用注解，使用简单
RxPermissions(9.7k) 需要RxJava2支持
easypermissions(8.5k)
AndPermissons(6.3k)严正杰出品


### ----2020.6.30（庚子年五月初十）Tuesday -----
Kotlin
var textViews: List<*>

Java
List<?> textViews;


[Kotlin中文社区](https://www.jianshu.com/u/a324daa6fa19)  

Kotlin协程依赖库导入
```
implementation 'org.jetbrains.kotlinx:kotlinx-coroutines-core:1.3.7'
implementation "org.jetbrains.kotlinx:kotlinx-coroutines-android:1.3.7" // Android
```
Kotlin切换线程
Dispatcher.dispatch切UI线程里面还是用的handler.post(runnable)
DefaultDispatcher-Worker-序数


Kotlin挂起线程
根据kotlin bytecode用到switch

kotlinx.coroutines提供的协程调度器包括：

Dispatchers.Default： 使用共享的后台线程池
Dispatchers.IO：用于IO操作的协程
Dispatchers.Unconfined：用于不消耗CPU时间的任务以及不更新UI的协程
用newSingleThreadContext创建的调度器：为协和的运行启动了一个线程，（一个专用的纯种是一种非常昂贵的资源）
[【Kotlin】协程(之二）](https://blog.csdn.net/menghaocheng/java/article/details/105320870)  



协程用法
launch+withContext

suspend fun ioFun1(){
	//withContext(Dispatchers.IO){
	withContext(Dispatchers.Default){
	 println("Coroutines Camp ioFun1 ${Thread.currentThread().name}")
	}
}

结构化并发
Coroutine Cancellation and Structured Concurrency

KTX扩展

CoroutineScope.launch{}
MainScope.launch{}
GlobalScope.launch{}
GlobalScope.launch(Dispatchers.Main){}
ViewModelScope.launch{}
LiveDataScope.launch{}
LifeCycleScope.launch{}
LifeCycleScope.launchWhenResumed{}


Kotlin协程delay比Thread.sleep性能更好


协程就是线程框架
kotlin的线程该不是轻量级的线程，只是线程框架
协程实质就是线程, 协程是线程的框架.

	fun click（view: View):Job = runBlocking{//外协程
		launch(Dispatchers.IO){//内协程
		Log.e("tag","launch $
		
		}
	}
	
	job.cancel()
```
suspend fun test6(){

    withContext ( Dispatchers.Main){
        println("Dispatchers.Main------"+ Thread.currentThread().name)
    }

    withContext(Dispatchers.IO) {
        println("Dispatchers.IO------"+ Thread.currentThread().name)
    }
}
````


【Kotlin协程简化理解】：
	线程池+线程切换
	用同步的方式写异步，消除回调

flutter连切换协程环境都不需要，只需要加两个关键字async和await


### ----2020.6.29（庚子年五月初九）Monday -----
云信下(公有)云升级问题排查到23点
儿子高烧至39.2℃

### ----2020.6.28（庚子年五月初八）Sunday -----
;--hava i been pwned?
https://haveibeenpwned.com/


### ----2020.6.27（庚子年五月初七）Saturday -----
职称论文还是未动笔
带儿子去玩儿童火车


### ----2020.6.26（庚子年五月初六）Friday -----


### ----2020.6.25（庚子年五月初五端午）Thursday -----
接待静静、计杨丽到访

Android源码设计模式解析与实战<第2版> 何红辉 关爱民 著
https://github.com/hehonghui


IModel
IView
IPresenter

BasePresenter<T>
	public class BasePresenter<T extends IView> implements IPresenter<T> {
	protected Reference<T> mView;
    protected BasePresenter<T> mPresenter;
    
    /**
     * 如果当前页面不需要操作数据,只需要 View 层,则使用此构造函数
     *
     * @param rootView
     */
    public BasePresenter(T rootView) {
        Preconditions.checkNotNull(rootView, "%s cannot be null", IView.class.getName());
        this.mView = new WeakReference<T>(rootView);
    }
    
    public BasePresenter() {
    
    }
    
    protected BasePresenter<T> getPresenter() {
        return this;
    }
    
    @Override
    public void attachView(T view) {
        if (mView == null) {
            mView = new WeakReference<T>(view);
        }
    }
    
    @Override
    public void detachView() {
        dispose();
        mView.clear();
        mView = null;
    }
    
    public T getView() {
        if (mView != null) {
            return mView.get();
        }
        return null;
    }



BaseActivity

	public abstract class BaseActivity<T extends IPresenter> extends AppCompatActivity implements IView {
	protected T mPresenter;
	
	protected void onCreate(@Nullable Bundle savedInstanceState) {
	    super.onCreate(savedInstanceState);
	    mContext = this;
	    ...
	    if (mPresenter != null) {
	        mPresenter.attachView(this);
	    }
	}
	
	protected void onDestroy() {
	    super.onDestroy();
	    if (mPresenter != null) {
	        mPresenter.detachView();
	        mPresenter = null;
	    }
	}


​	

### ----2020.6.24（庚子年五月初四）Wednesday -----
注解处理器
@SupportAnnotaionType
public CustomeAnnotationProcessor extends AbstractProcessor
	getSupportAnnotaionType()

resources/MEMA-INFO.services

annotationProcessor 引入注解
Filer filer = processingEnv.getFiler();
JavaFileObject javaFileObject = filer.createSourceFile("包名.类名");

	javaPreCompileDebug
	注：注解日志打印
	compileDebugJavaWithJavac

***
class1.isAssignableFrom(class2) 
class2是不是class1的子类或者子接口

***
SPI机制
PI全称Service Provider Interface

***
输入场景的页面变换(聊天输入框跳闪）PanelSwitchHelper 
https://juejin.im/post/5eddf8456fb9a04804041738

[PanelSwitchHelper✔️一个可帮助键盘平稳过渡到功能面板的框架](https://javascript.ctolib.com/yummylau-panelswitchhelper.html)  


### ----2020.6.23（庚子年五月初三）Tuesday -----

Kotlin协程：一个线程框架

kotlin：线程框架
launch+withContext
suspend标记

***
高效易用的加载反馈页管理框架 LoadSir 
[LoadSir](https://gitee.com/mirrors/LoadSir)  
LoadSir 是一个高效易用，低碳环保，扩展性良好的加载反馈页管理框架，在加载网络或其他数据时候，根据需求切换状态页面， 可添加自定义状态页面，如加载中，加载失败，无数据，网络超
https://www.oschina.net/p/loadsir

***
lottie
https://github.com/airbnb/lottie-android

***
BottomNavigationView底部导航栏




### ----2020.6.22（庚子年五月初二）Monday -----

【码上开学】--协程  
[学不会协程？很可能因为你看过的教程都是错的](https://www.bilibili.com/video/BV164411C7FK)  
[Kotlin 协程的挂起好神奇好难懂？今天我把它的皮给扒了](https://www.bilibili.com/video/BV1KJ41137E9)  
[到底什么是「非阻塞式」挂起？协程真的比线程更轻量级吗？](https://www.bilibili.com/video/BV1JE411R7hp)  




[强制Gradle 刷新依赖](https://www.jianshu.com/p/5e8e70f3c1d5)  
./gradlew :app:assembleDebug --refresh-dependencies
./gradlew assembleDebug --info

[gradlew常用命令](https://www.jianshu.com/p/be0d6445709d)  

***
公司maven私服  
http://10.1.193.100:8081/nexus/#welcome  

个人本地maven私服  
http://172.16.50.39:8081/artifactory/webapp/#/home  
                
	//url "http://10.1.193.100:8081/nexus/content/groups/Android/"
	url "http://172.16.50.39:8081/artifactory/android_group/"

***

[设计模式](https://www.runoob.com/design-pattern/design-pattern-tutorial.html)  


[微服务持续交付-系列课程](https://www.jfrogchina.com/series_webinars/)  


### ----2020.6.21（庚子年五月初一夏至）Sunday -----
凌晨2:30睡觉，眼睛干涩流泪不止  
学习使用frog-artifactory搭建本地私服  

[json字符串转pojo类](http://www.jsonschema2pojo.org/)  

***
[kotlin泛型](https://www.runoob.com/kotlin/kotlin-generics.html)  

where
对于多个上界约束条件，可以用 where 子句：
```
	fun <T> copyWhenGreater(list: List<T>, threshold: T): List<String>
		where T : CharSequence,
			  T : Comparable<T> {
		return list.filter { it > threshold }.map { it.toString() }
	}
```

Kotlin 泛型中的 in 和 out  协变

kotlin扩展函数
kotlin解构


### ----2020.6.20（庚子年闰四月廿九）Saturday -----
frog-artifactory搭建本地私服


### ----2020.6.19（庚子年闰四月廿八）Friday -----
代码分支合并失误

kotlin遍历打印1到100的数值
	for(index in 1..100){
         print(index)
    }



### ----2020.6.18（庚子年闰四月廿七）Thursday -----
java线程处理异常Thread.UncaughtExceptionHandler
    /**
     * 这个是最关键的函数，当程序中有未被捕获的异常，系统将会自动调用uncaughtException方法
     * thread为出现未捕获异常的线程，ex为未捕获的异常，有了这个ex，我们就可以得到异常信息
     */
    @Override
    public void uncaughtException(Thread thread, Throwable ex) {


第三方异常日志框架
谷歌BreakPad(Native日志)
腾讯bugly
XCrash（灵活自定义异常处理）
Sentry（日志过滤）

***

Spring容器：可看作里面一个Map，根据key可以取出对应的实例

***
[Android Studio（JAVA） 编译警告:使用了未经检查或不安全的操作](https://www.mobibrw.com/2015/2502)  
使用了未经检查或不安全的操作
要了解详细信息，请使用 "-Xlint:unchecked" 重新编译。
有关详细信息, 请使用 -Xlint:deprecation 重新编译。

注: 某些输入文件使用或覆盖了已过时的 API。
注: 有关详细信息, 请使用 -Xlint:deprecation 重新编译。


> Task :app:compileDebugJavaWithJavac  
注: D:\XXXX.java使用或覆盖了已过时的 API。  
注: 有关详细信息, 请使用 -Xlint:deprecation 重新编译。  
注: D:\XXXX.java使用了未经检查或不安全的操作。  
注: 有关详细信息, 请使用 -Xlint:unchecked 重新编译。  


```
     tasks.withType(JavaCompile) {
       options.compilerArgs << "-Xlint:unchecked"
     }
    
    
    //展示未检查与过时API详情信息
    gradle.projectsEvaluated {
         tasks.withType(JavaCompile) {
              options.compilerArgs << "-Xlint:unchecked" << "-Xlint:deprecation"
         }
    }


    final LinkedHashMap<WeakReference<Object>,WeakReference<Object>> aWeakArray = new LinkedHashMap<>();
    for (Iterator iter = aWeakArray.entrySet().iterator(); iter.hasNext(); ) {
        LinkedHashMap.Entry element = (LinkedHashMap.Entry)iter.next();
        WeakReference<Object> aWeakObj = (WeakReference<Object>)element.getKey();
        WeakReference<Object> aWeakTag = (WeakReference<Object>)element.getValue();
    }


    消除警告后的代码Java

    final LinkedHashMap<WeakReference<Object>,WeakReference<Object>> aWeakArray = new LinkedHashMap<>();
    for (Iterator<LinkedHashMap.Entry<WeakReference<Object>,WeakReference<Object>> > iter = aWeakArray.entrySet().iterator(); iter.hasNext(); ) {
        LinkedHashMap.Entry<WeakReference<Object>,WeakReference<Object>> element = iter.next();
        WeakReference<Object> aWeakObj = element.getKey();
        WeakReference<Object> aWeakTag = element.getValue();
    }

    final LinkedHashMap<WeakReference<Object>,WeakReference<Object>> aWeakArray = new LinkedHashMap<>();
    for (Iterator<LinkedHashMap.Entry<WeakReference<Object>,WeakReference<Object>> > iter = aWeakArray.entrySet().iterator(); iter.hasNext(); ) {
        LinkedHashMap.Entry<WeakReference<Object>,WeakReference<Object>> element = iter.next();
        WeakReference<Object> aWeakObj = element.getKey();
        WeakReference<Object> aWeakTag = element.getValue();
    }

```

### ----2020.6.17（庚子年闰四月廿六）Wednesday -----
vlayout阿里巴巴开源淘宝多布局LayoutManager库, a powerfull LayoutManager extension for RecyclerView

在一个RecyclerView中实现Grid、List等多样布局


[vlayout github](https://github.com/alibaba/vlayout)  
Project vlayout is a powerfull LayoutManager extension for RecyclerView, it provides a group of layouts for RecyclerView. 
Make it able to handle a complicate situation when grid, list and other layouts in the same recyclerview. http://tangram.pingguohe.net/

    LinearLayoutHelper: provide linear layout as LinearLayoutManager.
    GridLayoutHelper: provide grid layout as GridLayoutManager, but with more feature.
    FixLayoutHelper: fix the view at certain position of screen, the view does not scroll with whole page.
    ScrollFixLayoutHelper: fix the view at certain position of screen, but the view does not show until it scrolls to it position.
    FloatLayoutHelper: float the view on top of page, user can drag and drop it.
    ColumnLayoutHelper: perform like GridLayoutHelper but layouts all child views in one line.
    SingleLayoutHelper: contain only one child view.
    OnePlusNLayoutHelper: a custom layout with one child view layouted at left and the others at right, you may not need this.
    StickyLayoutHelper: scroll the view when its position is inside the screen, but fix the view at start or end when its position is outside the screen.
    StaggeredGridLayoutHelper: provide waterfall like layout as StaggeredGridLayoutManager.


### ----2020.6.16（庚子年闰四月廿五）Tuesday -----
去奉贤税务局


### ----2020.6.15（庚子年闰四月廿四）Monday -----

***

单词学习：
| tenured | 英[ˈtenjəd] | 美[ˈtenjərd] |
| ------- | ----------- | ------------ |
|         |             |              |

| adj. | 终身的; 长期保有的; 获终身聘用的; 享有终身职位的; |
| ---- | ------------------------------------------------- |
|      |                                                   |



[卫吴羡](https://blog.csdn.net/weixin_43258908)  

[卫吴羡RSS订阅]
https://blog.csdn.net/weixin_43258908/rss/list

***
TCP为何使用三次握手？Socket双向通信 REQ-ACK-SEQ-ACK



[Java程序启动时至少启动几个线程？](https://blog.csdn.net/Hope_lee/article/details/89645201)  

JMX的API

```
public class TestOne {
	public static void main(String[] args) {
		ThreadMXBean mxBean = ManagementFactory.getThreadMXBean();
		ThreadInfo[] allThreads = mxBean.dumpAllThreads(false, false);
		for (ThreadInfo threadInfo : allThreads) {
			System.out.println(threadInfo.getThreadId()+"==="+threadInfo.getThreadName());
			
		}
	}
}
```

输出的结果为：

5===Attach Listener 
4===Signal Dispatcher 分发处理发送给jvm信号的线程
3===Finalizer 调用对象finalize方法的线程，就是垃圾回收的线程
2===Reference Handler 清除reference的线程
1===main



***



[一个HelloWorld 的程序行这个应用，Java 至少会创建几个线程呢？](https://blog.csdn.net/weixin_43258908/article/details/89281773) 

在jdk8时，可见创建了5个线程。
main:主线程
Reference Handler：处理引用对象本身的垃圾回收
Finalizer：处理用户的Finalizer方法
Signal Dispatcher：外部jvm命令的转发器
Attach Listener: jvm提供一种jvm进程间通信的能力，能让一个进程传命令给另外一个进程



Windows应用程序开发工程师（有WinFrom、MFC、ASP.Net框架下的工作经验；）
Android应用程序开发工程师


【历史的鉴戒】
当下android app开发工程师的焦虑，可以参考当年windows应用程序开发工程师的焦虑和疑问

[自述内心深处的感想：5 Windows是否还有前途，是否需要深入学习Windows](https://www.cjjjs.com/article/201649141143294)  作者：王垠
[看了一篇讲述Windows程序员前途的文章有感而发转过来](https://blog.csdn.net/sesiria/article/details/77972783)  

***

[Windows API 参考手册](http://www.office-cn.net/t/api/api_content.htm)  


### ----2020.6.14（庚子年闰四月廿三）Sunday -----

ART从Android7.0使用混合编译

DVM基于寄存器



ART(AOT)预先编译

操作数栈-局部变量表



Zygote





### ----2020.6.13（庚子年闰四月廿二）Saturday -----

JVM垃圾回收算法：复制、标记清除、标记整理



Android使用CMS(Concurrent Mark Sweep)垃圾回收



### ----2020.6.12（庚子年闰四月廿一）Friday -----

马老师邮寄的

《马士兵多线程与高并发》2020年第一版

基本概念 * JUC同步工具 * 同步容器 * 

ClassLoader--loadClass---findClass

BaseDexClassLoader

PathClassLoader所有类都是

DexClassLoader JDK8与PathClassLoader合二为一

BootClassLoader











### ----2020.6.11（庚子年闰四月二十）Thursday -----

未记录



### ----2020.6.10（庚子年闰四月十九）Wednesday -----

***
[Java之JVM逃逸分析](https://blog.csdn.net/blueheart20/article/details/76167489)  

逃逸分析开启设置
默认的在JDK 6u23以上是默认开启，这里将设置重新明确一下：
强制开启：

	-server -XX:+DoEscapeAnalysis -XX:+PrintGCDetail -Xmx10m -Xms10m
	
	关闭逃逸分析：
	
	-server -XX:-DoEscapeAnalysis -XX:+PrintGCDetail -Xmx10m -Xms10m



### ----2020.6.9（庚子年闰四月十八）Tuesday -----
中级职称资料



### ----2020.6.8（庚子年闰四月十七）Monday -----

[设计模式之工厂模式（factory pattern）](https://www.cnblogs.com/yssjun/p/11102162.html)  
[Java学习笔记之UnaryOperator](https://blog.csdn.net/yangshuaionline/article/details/85329657)  

    package java.util.function;
    
    /**
     * Represents an operation on a single operand that produces a result of the
     * same type as its operand.  This is a specialization of {@code Function} for
     * the case where the operand and result are of the same type.
     *
     * <p>This is a <a href="package-summary.html">functional interface</a>
     * whose functional method is {@link #apply(Object)}.
     *
     * @param <T> the type of the operand and result of the operator
     *
     * @see Function
     * @since 1.8
     */
    @FunctionalInterface
    public interface UnaryOperator<T> extends Function<T, T> {
    
        /**
         * Returns a unary operator that always returns its input argument.
         *
         * @param <T> the type of the input and output of the operator
         * @return a unary operator that always returns its input argument
         */
        static <T> UnaryOperator<T> identity() {
            return t -> t;
        }
        
    }
    
    //identity方法的等价写法
    static <T> UnaryOperator<T> identity() {
        //代码return t -> t;的等价写法如下
        return new UnaryOperator<T>() {
            @Override
            public T apply(T t) {
               return t;
            }
        };
    }

英语补习
operand  ['ɑpə'rænd /'ɒpərænd]
n.  运算域, 数学操作运算的量; 用于操作的数据单位 (数学, 计算机用语)

[进程间通信IPC、LPC、RPC](https://www.cnblogs.com/gsk99/archive/2010/12/13/1904541.html)  
IPC:(Inter-Process Communication)跨进程通信:进程间通信技术包括"消息传递、同步、共享内存和远程过程调用"。  
LPC:(Local Procedure Call)本地过程调用
RPC:(Remote Procedure Call)远程过程调用  


[JDK1.9对Optional类的改进，ifPresentOrElse() 方法](https://blog.csdn.net/qq_35951897/article/details/97780993)  


### ----2020.6.7（庚子年闰四月十六）Sunday -----
https://docs.oracle.com/javase/8/docs/technotes/tools/unix/java.html

Class文件中除了有类的版本、字段、方法、接口等描述信息外，还有一项信息就是常量池，用于存放 编译时期生成的各种字面量和符号引用，这部分内容将在类加载后进入方法区的运行时常量池中存放。
按照系統改變
https://docs.oracle.com/javase/8/docs/technotes/tools/unix/java.html#BABCBGHF


方法区：
JDK1.7之前称为永久代
JDK1.8之后称为元空间


方法区是虚拟机规范, 是概念的东西, 1.7用永久代实现方法去, 1.8用元空间实现永久代
方法区在JDK 8中就是Metaspace，在JDK6或7中就是Perm Space


-Xmx200M（堆区内存可被分配的最大上限	10G
-Xms 堆区内存初始内存分配的大小			2G

Oracle：1、hotspot	2、JRocket（没有永久代）

直接内存
directByteBuffer



方法区
栈区、堆、本地内存


eden s0 s1 tenured permanent

ps -ef|grep java

**HSDB**


**共享区域为什么分为堆和方法区？**
堆里面会有变化，会有GC，  
方法区几乎不变，Class加载一次基本就不变了  

**第33条：优先考虑类型安全的异构容器**
类型令牌（type token）
String.class属于Class<String>类型
Integer.class属于Class<Integer>类型

	public class Class<T> {
		T cast(Object obj);
	}


**第60条：如果需要精确的答案，请避免使用float和double**
请使用BigDecimal、int或者long进行  货币运算(float和double类型尤其不适合用于货币计算，主要用于科学计算和工程计算）

java是伪泛型(编译时泛型,运行时类型擦除(type erasure))，真泛型语言如C#、 C++（模板）
协变(covariant):数组是协变的（covariant）。这就是说如果sub是super的子类型，那么数组类型sub[]就是super[]的子类型。  
逆变(contravariant)
不变(invariant)：泛型是不可变的（invariant），对于任意两个不同的类型type1和type2，List<type1>既不是List<type1>的子类型，也不是List<type2>的超类型。

***
C++模板是"reified generic"

reify
verb [ T ]
  formal
UK/ˈreɪ.ɪ.faɪ/ US/ˈriː.ə.faɪ/
to make something more real or consider it as real
使物体化；使具体化
***

* 任何情况下都不要在多个线程间共享一个Random实例，而该把它放入ThreadLocal之中
* java7 **在所有情形下** 都更推荐使用ThreadLocalRandom，它向下兼容已有的代码且运营成本更低
	
	ThreadLocalRandom的主要实现细节：
	* 使用一个普通的long而不是使用Random中的AtomicLong作为seed
	* 不能自己创建ThreadLocalRandom实例，因为它的构造函数是私有的，可以使用它的静态工厂ThreadLocalRandom.current()
	* 它是CPU缓存感知式的，使用8个long虚拟域来填充64位L1高速缓存行

***
predicate
美: ['predɪkeɪt] 
英: ['predɪkət] 
v.	断言；使基于；使以…为依据；表明
adj.	述语的；谓项的
n.	谓语（句子成分，对主语加以陈述，如 John went home 中的 went home）
网络	谓词；述词；断定


negate
美: [nə'ɡeɪt] 
英: [nɪ'ɡeɪt] 
v.	否定；否认；取消；使无效
网络	非；打消；抵消



### ----2020.6.6（庚子年闰四月十五）Saturday -----

Effective Java<Third Edition> Joshua Bloch 俞黎敏译

**第30条：优先考虑泛型方法**  
递归类型限制(recursive type bound)  
	
	//Using a recursive type bound to express mutual comparability(集合元素可以互相比较）
	public static <E extends Comparable<E>> E max(Collection<E> c)

**第42条：Lambda优先于匿名类**

**第43条：方法引用优先于Lambda**

**第44条：坚持使用标准的函数接口**
unary (adj.)一元的
1923, from Latin unus "one" (from PIE root *oi-no- "one, unique") on model of binary, etc.

|		接口		|	函数签名		|		范例		|
|-------------------|-------------------|-------------------|
| UnaryOperator<T>	|T apply(T t)		|String::toLowerCase|
| BinaryOperator<T>	|T apply(T t1,T t2)	|BigInteger::add	|
| Predicate<T>		|booean test(T t)	|Collection::isEmpty|
| Function<T,R>		|R apply(T t)		|Arrays::asList		|
| Supplier<T>		|T get()			|Instant::now		|
| Consumer<T>		|void accept(T t)	|System.out::println|

***
1.8的新特性—>函数式编程即:将函数作为参数

	java.util
		Class Objects
		java.lang.Object
		java.util.Objects
	
	static <T> T	requireNonNull(T obj)
	Checks that the specified object reference is not null.
	static <T> T	requireNonNull(T obj, String message)
	Checks that the specified object reference is not null and throws a customized NullPointerException if it is.

***
[马士兵教育：SpringBoot学习](https://gitee.com/freedomszq/shiro.git)  



### ----2020.6.5（庚子年闰四月十四）Friday -----

[正则表达式校验网址](http://leaverou.github.io/regexplained/)  

[json在线格式化](https://www.sojson.com/)  


[在线颜色选择器 | RGB颜色查询对照表](http://tools.jb51.net/static/colorpicker/?)  


**mybase**  
[个人（wiki）知识管理工具-一代神器之mybase](http://www.eryajf.net/1040.html)  


### ----2020.6.4（庚子年闰四月十三）Thursday -----
com.google.gson.reflect.TypeToken获取运行时泛型类型(参数化类型)

***
hightopo是一款收费软件,它可以很方便的帮助我们制作web版的网络拓扑图。它的底层是 HTML5 的 Canvas 实现。
[大型风力发电机-在线三维动图](https://hightopo.com/demo/fan3d-magic/)  

***
[泛型与通配符详解](https://www.cnblogs.com/fengmingyue/p/6087031.html)  

    public void fun3() {
        List<Integer> intList = new ArrayList<Integer>();
        print1(intList);
        List<Long> longList = new ArrayList<Long>();
        print1(longList);
    }
    /*
     * 给通配符添加了限定：
     *   只能传递Number或其子类型
     *   子类通配符对通用性产生了影响，但使用形参更加灵活
     */
    public void print1(List<? extends Number> list) {
        //list.add(new Integer(100));//错误！！！编译器报错，说明参数为泛型的方法还是不能使用（因为?也可能为Long型）
        Number number = list.get(0);//正确！！！返回值为泛型的方法可用了！
    }


​    
​    public void fun4() {
​        List<Integer> intList = new ArrayList<Integer>();
​        print2(intList);
​        List<Number> numberList = new ArrayList<Number>();
​        print2(numberList);
​        List<Object> objList = new ArrayList<Object>();
​        print2(objList);
​    }
​    /*
​     * 给通配符添加了限定
​     *   只能传递Integer类型，或其父类型
​     */
​    public void print2(List<? super Integer> list) {
​        list.add(new Integer(100));//正确！！！参数为泛型的方法可以使用了
​        Object obj =  list.get(0);//正确！！！但是只是得益于object类是所有类的父类，换成其他任何类编译器都会报错！说明返回值为泛型的方法，还是不能使用
​    }


### ----2020.6.3（庚子年闰四月十二）Wednesday -----

***

参数化类型(parameterized types)具体含义:
在List<Sting>中，String 就是参数化类型；

类型变量（type variables）具体含义：
List<T> list中，T就是类型变量


	package java.lang.reflect;
	
	/**
	 * Type is the common superinterface for all types in the Java
	 * programming language. These include raw types, parameterized types,
	 * array types, type variables and primitive types.
	 *Type是 Java 编程语言中所有类型的公共高级接口。它们包括原始类型、参数化类型、数组类型、类型变量和基本类型。
	 * @since 1.5
	 */
	
	public interface Type {



***
[Java 获取泛型对象的参数类型](https://blog.csdn.net/Gdeer/article/details/104591155/)  
由于类型擦除，java 中的泛型对象在运行时是不知道自己类型参数的类型的。
但有几种特殊情况，能够获取泛型对象的参数类型：

	一、类中有 class 信息（类中有一个 Class 字段）
	二、父类中有 class 信息（父类是泛型类，并指定了参数类型）
		2.1 子类
		2.2 匿名子类
	三、持有者中有 class 信息（是一个类的 Field、Method）


### ----2020.6.2（庚子年闰四月十一）Tuesday -----
装饰器模式
File)FileInputStream)FilterInputStream)BufferInputStream)DataInputStream


### ----2020.6.1（庚子年闰四月初十）Monday -----
* 概念---逆波兰 表达式

装饰器模式（洋葱模型）
[RxJava2线程调度](https://xieyang94.github.io/RxJava-/RxJava2/RxJava2-%E7%BA%BF%E7%A8%8B%E8%B0%83%E5%BA%A6.html)  



### ----2020.5.31（庚子年闰四月初九）Sunday -----
**TypeToken**
[关于Gson的TypeToken](https://www.jianshu.com/p/c820e55d9f27)  
​ Gson在Json解析中使用广泛, 常用的数据类型都可以解析, 特殊的可以自定义Adapter解析. 在解析大量具有某些相同结构的数据上,我们总想复用已有的类型, 为了复用通常可以使用继承和泛型

***
[Gson中使用TypeAdapter设置默认值, 数据免判空、解析后校验、预处理](https://ubock.com/article/45)  
Gson中使用TypeAdapter设置默认值，如数字类型Long默认是null,但是我们需要0



### ----2020.5.30（庚子年闰四月初八）Saturday -----
RxJava装饰器模式（洋葱模型） 

Binder



### ----2020.5.29（庚子年闰四月初七）Friday -----
[高并发编程之AtomicReference讲解](https://blog.csdn.net/weixin_42146366/article/details/87822781)  
一、AtomicReference介绍  
①.AtomicReference和AtomicInteger非常类似，不同之处就在于AtomicInteger是对整数的封装，而AtomicReference则对应普通的对象引用。也就是它可以保证你在修改对象引用时的线程安全性。  
②.AtomicReference是作用是对”对象”进行原子操作。 提供了一种读和写都是原子性的对象引用变量。原子意味着多个线程试图改变同一个AtomicReference(例如比较和交换操作)将不会使得AtomicReference处于不一致的状态。  

***
[大端和小端存储模式详解](https://www.cnblogs.com/still-smile/p/11595775.html)  
**什么是大端和小端**
Big-Endian和Little-Endian的定义如下：
1) Little-Endian就是低位字节排放在内存的低地址端，高位字节排放在内存的高地址端。
2) Big-Endian就是高位字节排放在内存的低地址端，低位字节排放在内存的高地址端。
举一个例子，比如数字0x12 34 56 78在内存中的表示形式为：
1)大端模式：
低地址 -------------> 高地址
0x12  |  0x34  |  0x56  |  0x78
2)小端模式：
低地址 ----------> 高地址
0x78  |  0x56  |  0x34  |  0x12
可见，大端模式和字符串的存储模式类似。

具体例子：
16bit宽的数0x1234在Little-endian模式（以及Big-endian模式）CPU内存中的存放方式（假设从地址0x4000开始存放）为：

|内存地址 | 小端模式存放内容 | 大端模式存放内容 |
|------  |-------------  |-------------- |
|0x4000  |    0x34       |      0x12     |
|0x4001  |    0x12       |      0x34     |

***


### ----2020.5.28（庚子年闰四月初六）Thursday -----

javassist


rxjava

**RxJavaPlugins**

RxJavaPlugins.onAssembly

[RxjavaPlugins](https://blog.csdn.net/weixin_43724742/article/details/103394113)  





### ----2020.5.27（庚子年闰四月初五）Wednesday -----
[《我们一起进大厂》系列-HashMap](https://juejin.im/post/5dee6f54f265da33ba5a79c8)
[DVM，应用程序的进程，Linux的进程](https://blog.csdn.net/lin111000713/article/details/52459710)  
**DVM的进程和Linux的进程, 应用程序的进程为同一个概念**
* DVM的进程
* Linux的进程
* 应用程序的进程

DVM指dalivk的虚拟机。
每一个【Android应用程序】都在它自己的进程中运行，都拥有一个【独立的Dalvik虚拟机实例】。
而每一个【DVM】都是【在Linux中的一个进程】，所以说可以认为是同一个概念




模板方法模式 VS 工厂方法模式

钩子线程

**JDK1.6与1.7有什么区别？**

***
Gson课程干货：
javabean类中的注解，key名，是否参与序列化，版本号；
原理，词法分析，构词规则，解析流程，自定义TypeAdapter，
自定义实现JsonDeserializer接口，TypeToken，nullSafe，nextNull，
设计模式等的




### ----2020.5.26（庚子年闰四月初四）Tuesday -----
[Android刘海屏、水滴屏全面屏适配方案](https://www.jianshu.com/p/2b8db60ba8df)  
[Android刘海屏、水滴屏等全面屏适配工具](https://github.com/smarxpan/NotchScreenTool)  

[Android 最佳并发实践之基础篇](https://mp.weixin.qq.com/s/jo142pIuknpECf6O7yb6DA)  
[看完，这辈子都忘不了责任链模式](https://mp.weixin.qq.com/s/0tyFKaHllRsawt3c56UGXg)  
[Wake up , 您有一条新的消息等待查收！](https://mp.weixin.qq.com/s/kA0-42fiL_oHQXruA8pfPw)  



[并发编程系列：面试官最想要的synchronized，你值得拥有](https://mp.weixin.qq.com/s/zi0A4kZgnjnF2-XtAi4pxQ)  
[关于多线程，你必须知道的那些玩意儿](https://mp.weixin.qq.com/s/QNeM3kuUZkicJVWjraDzQA)  
[单例的线程安全及序列化问题](https://mp.weixin.qq.com/s/p-4gC9TDSOxQPTJLou-s-w)  



### ----2020.5.25（庚子年闰四月初三）Monday -----

[Android获取屏幕高度的坑](https://www.jianshu.com/p/74a7a40437cb)  

***
[FrameLayout 配合ImageView 设置背景](https://blog.csdn.net/a15140288018/article/details/84294933)  
	
	<FrameLayout
		android:layout_width="match_parent"
		android:layout_height="match_parent" >
		<ImageView
			android:layout_width="match_parent"
			android:layout_height="match_parent"
			android:background="@drawable/login_title_bg" />
		//不可将"background"换成"src"属性，这样会引发ImageView无法完全填充FrameLayout。


​		
### ----2020.5.24（庚子年闰四月初二）Sunday -----
Gson
TypeAdapter(适配器模式）
TypeToken
JsonDeserializer
Gson.fromJson(String json,Class clazz)(门面模式、代理模式）
[Gson实现自定义解析json格式](https://www.cnblogs.com/xiaowangabc/p/d0c34013b6c24a4f62a3bdedb3b0a5cc.html)  
JsonParser  解析json文本的解析器，它将json文本解析成JsonElement树。  
JsonElement 用来表示一个json元素的类，它可能是JsonObject,JsonArray,JsonPrimitive,JsonNull.  


### ----2020.5.23（庚子年闰四月初一）Saterday -----
//用于判断当前线程是否运行在主线程
Looper.mylooper()==Looper.mainLooper();

[Android判断当前是否在主线程](https://www.cnblogs.com/genggeng/p/7524948.html)

	public boolean isMainThread() {
		return Looper.getMainLooper() == Looper.myLooper();
	}


​	
​	public boolean isMainThread() {
​		return Looper.getMainLooper().getThread() == Thread.currentThread();
​	}


	public boolean isMainThread() {
		return Looper.getMainLooper().getThread().getId() == Thread.currentThread().getId();
	}

***
***加班升级--还是遗留了bug（网点支付宝不能维护）git多分支管理不善惹得祸


### ----2020.5.22（庚子年四月三十）Friday -----

[Android Bitmap 详解：关于 Bitamp 你所要知道的一切](https://www.jianshu.com/p/eef3daeeecbc)
[Android 最佳并发实践之基础篇](https://mp.weixin.qq.com/s/jo142pIuknpECf6O7yb6DA)

***
[并发编程系列：面试官最想要的synchronized，你值得拥有](https://mp.weixin.qq.com/s/zi0A4kZgnjnF2-XtAi4pxQ)
[java单例模式之readResolve()，在序列化&反序列化时保持单例](https://blog.csdn.net/u011499747/article/details/50982956)  

	import java.io.Serializable;
	import java.util.Objects;
	public class SerSingleton implements Serializable {
		String name;
		private SerSingleton(){
			System.out.println("Singleton is creating");
		}
	
		private static SerSingleton instance = new SerSingleton();
	
		public static SerSingleton getInstance(){
			return instance;
		}
	
		public static void createString(){
			System.out.println("create string in singleton");
		}
	
		private Object readResolve(){
			System.out.println("read resolve");
			return instance;
		}
	}
***

### ----2020.5.21（庚子年四月廿九）Thursday -----
感谢神，赐下灵感解决麻烦问题，保准生产应用稳定准时上线--


### ----2020.5.20（庚子年四月廿八）Wednesday -----
身份证正反面识别，身份证扫描识别，二代身份证OCR识别，OCR极速识别身份证所有信息正反面均可。离线无需联网,极速秒扫。
https://github.com/XieZhiFa/IdCardOCR


[0 UI颜色渐变效果](https://uigradients.com/#Flickr)  
[1 Android开发网址导航](http://www.jcodecraeer.com/hao.html#)  
[2 程序员导航](https://playmei.com/developer.html)  
[3 GIFFOX技术资源站点](http://code.giffox.com/)  
[4 极客文档](https://geekdocs.cn/)  
[5 开源中国](https://www.oschina.net/)  

[为了在简历上写掌握Java多线程和并发编程，做了两万字总结！！！](https://blog.csdn.net/HeZhiYing_/article/details/105943962?utm_source=app)  
[Android面试点](https://github.com/zytc2009/Android_learning/tree/master/%E9%9D%A2%E8%AF%95%E9%A2%98/android%E9%9D%A2%E8%AF%95%E7%82%B9)  

[Android内核设计思想](http://mp.weixin.qq.com/mp/homepage?__biz=MzA5OTAxNDEyNg==&hid=1&sn=ebe1c61ff758e51e9e92fd907a99f342&scene=18#wechat_redirect)  
[约束布局ConstraintLayout看这一篇就够了](https://www.jianshu.com/p/17ec9bd6ca8a)  


[kotlin中文学习](http://www.kotlincn.net/docs/reference/basic-syntax.html)

***
android 4.4以上沉浸式状态栏和沉浸式导航栏管理，适配横竖屏切换、刘海屏、软键盘弹出等问题，可以修改状态栏字体颜色和导航栏图标颜色，以及不可修改字体颜色手机的适配，适用于Activity、Fragment、DialogFragment、Dialog，PopupWindow，一句代码轻松实现，以及对bar的其他设置
[沉浸式状态栏&导航栏](https://github.com/gyf-dev/ImmersionBar)

***
LinkedBlockingQueue  代码实现阻塞细节-->ReentrantLock

    /** Main lock guarding all access */
    final ReentrantLock lock = new ReentrantLock();
    
    /** Condition for waiting takes */
    private final Condition notEmpty = lock.newCondition();
    
    /** Condition for waiting puts */
    private final Condition notFull = lock.newCondition();

***
[线程池，这一篇或许就够了](https://mp.weixin.qq.com/s/r_7EsctIudMb0O5-FNIWmQ)  

***
[线程池 8 大拒绝策略，别说你不会！](https://mp.weixin.qq.com/s/nPe253SsKkBFhZPmFKoD1w)  
    
    public interface RejectedExecutionHandler {
        void rejectedExecution(Runnable r, ThreadPoolExecutor executor);
    }

【8大拒绝策略】=JDK预设的4种线程池拒绝策略+四款第三方拒绝策略实现
**JDK内置实现**  
    CallerRunsPolicy（调用者运行策略）  
    AbortPolicy（中止策略）  
    DiscardPolicy（丢弃策略）  
    DiscardOldestPolicy（弃老策略）  
**第三方实现**  
    dubbo中的线程拒绝策略  
    Netty中的线程池拒绝策略  
    activeMq中的线程池拒绝策略  
    pinpoint中的线程池拒绝策略  

***
[java阻塞队列与非阻塞队列](https://blog.csdn.net/danengbinggan33/article/details/73105838)
[Java中常用七个阻塞队列的总结](https://www.cnblogs.com/kaigejava/p/12825493.html)  

方法\处理方式	抛出异常	返回特殊值	一直阻塞	超时退出
插入方法	add(e)	offer(e)	put(e)	offer(e,time,unit)
移除方法	remove()	poll()	take()	poll(time,unit)
检查方法	element()	peek()	不可用	不可用

**阻塞队列**
JDK7提供了7个阻塞队列。分别是：
ArrayBlockingQueue ：一个由数组结构组成的有界阻塞队列。
LinkedBlockingQueue ：一个由链表结构组成的有界阻塞队列。
PriorityBlockingQueue ：一个支持优先级排序的无界阻塞队列。
DelayQueue：一个使用优先级队列实现的无界阻塞队列。
SynchronousQueue：一个不存储元素的阻塞队列。
LinkedTransferQueue：一个由链表结构组成的无界阻塞队列。
LinkedBlockingDeque：一个由链表结构组成的双向阻塞队列。

**非阻塞队列**
LinkedList（java中的LinkedList 是采用双向循环列表实现的。利用LinkedList 可以实现栈（stack）、队列（queue））
PriorityQueue
ConcurrentLinkedQueue

***
**Queue和List区别&联系**
联系
public interface Queue<E> extends Collection<E> {
public interface List<E> extends Collection<E> {

双方共同继承自Collection接口
public interface Collection<E> extends Iterable<E> {

java.util.Collection#add(E)  
java.util.Collection#addAll(Collection<? extends E>)  
java.util.Collection#clear  
java.util.Collection#contains  
java.util.Collection#containsAll  
java.util.Collection#isEmpty  
java.util.Collection#parallelStream  
java.util.Collection#remove  
java.util.Collection#removeAll  
java.util.Collection#removeIf  
java.util.Collection#retainAll  
java.util.Collection#size  
java.util.Collection#stream  
java.util.Collection#toArray()  
java.util.Collection#toArray(T[])  


|   Queue           |   List    |
|-------------------|-----------|
|   element:E       |   add     |
|   offer(E):boolean|   remove  |
|   peek:E          |   get     |
|   poll:E          |   set     |
|   remove:E        |   add     |

***
***添加元素***

    /**
     * Inserts the specified element into this queue if it is possible to do
     * so immediately without violating capacity restrictions.
     * When using a capacity-restricted queue, this method is generally
     * preferable to {@link #add}, which can fail to insert an element only
     * by throwing an exception.
     *
     * @param e the element to add
     * @return {@code true} if the element was added to this queue, else
     *         {@code false}
     * @throws ClassCastException if the class of the specified element
     *         prevents it from being added to this queue
     * @throws NullPointerException if the specified element is null and
     *         this queue does not permit null elements
     * @throws IllegalArgumentException if some property of this element
     *         prevents it from being added to this queue
     */
    boolean offer(E e);

****下面为获取元素****
    
    /**
     * Retrieves, but does not remove, the head of this queue.  This method
     * differs from {@link #peek peek} only in that it throws an exception
     * if this queue is empty.
     *
     * @return the head of this queue
     * @throws NoSuchElementException if this queue is empty
     */
    E element();
    
    /**
     * Retrieves, but does not remove, the head of this queue,
     * or returns {@code null} if this queue is empty.
     *
     * @return the head of this queue, or {@code null} if this queue is empty
     */
    E peek();
    
    /**
     * Retrieves and removes the head of this queue,
     * or returns {@code null} if this queue is empty.
     *
     * @return the head of this queue, or {@code null} if this queue is empty
     */
    E poll();
    
    /**
     * Retrieves and removes the head of this queue.  This method differs
     * from {@link #poll poll} only in that it throws an exception if this
     * queue is empty.
     *
     * @return the head of this queue
     * @throws NoSuchElementException if this queue is empty
     */
    E remove();


**Queue  VS BlockingQueue**
public interface Queue<E> extends Collection<E> {

public interface BlockingQueue<E> extends Queue<E> {  
put(E):void  
take():E  
offer(E,long,TimeUnit):boolean  
poll(long,TimeUnit):E  




### ----2020.5.19（庚子年四月廿七）Tuesday -----

[应届生/社招面试最爱问的几道Java基础问题](https://juejin.im/post/5e18879e6fb9a02fc63602e2)  

[java字节码速查表](https://www.wanandroid.com/blog/show/2277)  


android打包  
terminal输入指令编译
编译release包
./gradlew assembleRelease  
./gradlew assembleUat

***
Java8伪共享和缓存行填充--@Contended注释

cache line（缓存行） 64byte
伪共享

jvm：设置-XX:RestrictContended
@sun.misc.Contended


[线程基础：多任务处理（18）——MESI协议以及带来的问题：伪共享](https://www.cnblogs.com/liulaolaiu/p/11744225.html)  
**MESI 协议**
* M（修改，Modified）：本地处理器已经修改缓存行，即是脏行，它的内容与内存中的内容不一样，并且此 cache 只有本地一个拷贝(专有)；
* E（专有，Exclusive）：缓存行内容和内存中的一样，而且其它处理器都没有这行数据；
* S（共享，Shared）：缓存行内容和内存中的一样, 有可能其它处理器也存在此缓存行的拷贝；
* I（无效，Invalid）：缓存行失效, 不能使用。

**RFO请求（Request For Owner）**


### ----2020.5.18（庚子年四月廿六）Monday -----
* GC ROOTS内存回收(对象回收）
1. 线程栈变量【虚拟机栈（栈帧中的局部变量区，也叫局部变量表）)】
2. 静态变量【方法区中的类静态属性引用的对象】
3. 方法区中常量引用
4. 本地方法栈JNI（Native）方法引用


**3种GC Algorithms**
* Mark-Sweep（标记清除）
* Copying（拷贝）
* Mark-Compact(标记压缩）

**垃圾回收器
Serial Old
stop-the-world

CMS:concurrent mark sweep


 OldTenured:年老代年轻代的对象如果能够挺过数次收集,就会进入老人区。 
 -XX:MaxTenuringThreshold=设置熬过年轻代多少
 -XX:MaxTenuringThreshold设置的是年龄阈值，默认15（对象被复制的次数）


**Java 的内存模型分**
* Young（年轻代）
* Tenured（终身代）
* Perm（永久代）

有些旧版本也叫作
* New
* Old
* Perm

* Eden区
* Tenured区
* Perm区





永久代的初始值-XX:PermSize及最大值-XX:MaxPermSize应该比永久代活跃数据大1.2~1.5倍
-XX:PermSize=13m，-XX:MaxPermSize=13m
java -Xms200m -Xmx200M -XX:+PrintGC com.mashibing.java.gc.T15FullGCProblem
 -Xms200m -Xmx200M 防止内存抖动

新生代大量死去，少量存活，采用复制算法
老年代存活率高，回收较少，采用MC或MS

top命令查看线程信息和jstack使用介绍

jstack定义： jstack是java虚拟机自带的一种堆栈跟踪工具。
top -Hp pid
top pstack ps -eaf


jmap -histo
dump+jmap分析



***
Jconsole （Java Monitoring and Management Console），一种基于JMX的可视化监视、管理工具。
jvisualvm远程连接监控
MAT内存分析工具(Memory Analyzer Tool)

**JProfiler是由ej-technologies GmbH公司开发的一款性能瓶颈分析工具(该公司还开发部署工具)。
其特点:

使用方便
界面操作友好
对被分析的应用影响小
CPU,Thread,Memory分析功能尤其强大
支持对jdbc,noSql, jsp, servlet, socket等进行分析
支持多种模式(离线，在线)的分析

**Arthas - Java 线上问题定位处理的终极利器
排查 Java 线上问题时，如 CPU 飙升、负载突高、内存溢出等问题，你需要查命令，查网络，然后 jps、jstack、jmap、jhat、jstat、hprof 等一通操作

dashboard指令
thread -b//查看线程死锁

jmap -histo pid | head -20

top+jstack


Full GC
***

CyclicBarrier(int parties,Runable barrierAction);//runable:达到屏障点要做的事情
await()：进行阻塞直到线程数达到屏障点
await(timeout)
geNumberWaiting();//获取正在CyclicBarrier上等待的线程数

CyclicBarrier.Generation ge


juc.locks.ReentrantLock
juc.locks.StampedLock
juc.locks.LockSupport
juc.Semaphore
juc.Phaser


java.util.concurrent.locks.AbstractQueuedSynchronizer extends java.util.concurrent.lock.AbstractOwnableSynchronizer

java.util.concurrent.locks.Condition

	    public class ConditionObject implements Condition, java.io.Serializable {
	    private static final long serialVersionUID = 1173984872572414699L;
	    /** First node of condition queue. */
	    private transient Node firstWaiter;
	    /** Last node of condition queue. */
	    private transient Node lastWaiter;


Sync

***
LockSupport(AQS)





***
IPC（Inter-Process Communication）
AIDL(Android interface Definition Language)

android.os.IBinder

最好异步加上oneway

AMS---ActivityManagerService
android.app.ActivityManagerNative.getDefault().bindService()-->IActivityManager
ServiceManager本身是一个进程

IServiceConnection

Client-AMS-Service



广播进程间通信--底层原理-->使用Binder实现
四大组件--底层通信--Binder
进程之间通信--Binder
native驱动 ---  Messenger
***
zygote进程和system server进程通信 为啥用socket 而不用binder 进行线程通信?
***
[AIDL与Binder与Messenger的使用区别！](https://blog.csdn.net/luojiusan520/article/details/50840008)
适用范围 messenger<binder<aidl  

### ----2020.5.17（庚子年四月廿五）Sunday -----

***
AQS(AbstractQueuedSynchronizer)
提供FIFO队列，是一个用来实现同步锁以及其他涉及到同步功能的核心组件，常见的有:ReentrantLock、CountDownLatch等。
AQS是一个抽象类，主要是通过继承的方式来使用，它本身没有实现任何的同步接口，仅仅是**定义了同步状态的获取以及释放的方法**来提供自定义的同步组件
CLH CLH(Craig, Landin, and Hagersten locks): 是一个自旋锁，能确保无饥饿性，提供先来先服务的公平性。
CLH锁也是一种基于链表的可扩展、高性能、公平的自旋锁，申请线程只在本地变量上自旋，它不断轮询前驱的状态，如果发现前驱释放了锁就结束自旋。
链接：https://www.jianshu.com/p/4682a6b0802d
***


Glide LRU缓存 算法实现->
	LinkedHashMap(int initialCapacity, float loadFactor, boolean accessOrder)
https://blog.csdn.net/a724888/article/details/80290276


[实现LRU算法的两种方法](https://blog.csdn.net/Apple_hzc/article/details/84640879)  
* 一、LinkedHashMap
	LinkedHashMap 内部维护了一个双向链表，用来维护插入顺序或者 LRU（最近最久未使用）顺序。
	* 设定最大缓存空间 threshold 为4；
	* 使用 LinkedHashMap 的构造函数将 accessOrder 设置为 true，开 LRU 顺序；
	* 覆盖 removeEldestEntry()方法实现，在结点多于 threshold 时就会将最近最久未使用的数据移除。

         private static final int MAX_ENTRIES = 100;
          
         protected boolean removeEldestEntry(Map.Entry eldest) {
            return size() > MAX_ENTRIES;
         }	

* 二、双向链表 + HashMap


threshold
美: ['θreʃ.hoʊld] 
英: ['θreʃ.həʊld] 
n.	阈；门槛；起点；开端
网络	阈值；阀值；临界值

***

netty粘包
https://blog.csdn.net/crazymakercircle/article/details/83957259

***
* 类加载为什么要使用双亲委派？主要是由于安全(java.lang.String)，另外基于效率原因，上级已经加载就不用再次加载了
Custom ClassLoader-->AppClassLoader(classpath)-->Extension ClassLoader(ext)-->Bootstrap

System.getProperty("sun.boot.class.path");
%JAVA_HOMR%/bin/
%JAVA_HOMR%/jre

System.getProperty("java.ext.dirs");
%ext
System.getProperty("java.class.path");

sun.misc.launcher$AppClassLoader@18b4aac3
sun.misc.launcher$ExtClassLoader@4554617c


双亲委派：自底向上，然后自顶向下返回


### ----2020.5.16（庚子年四月廿四）Saturday -----
Retrofit(okhttp)  
enqueue异步执行  
execute()同步执行  

单链表反转：pre、next  



### ----2020.5.15（庚子年四月廿三）Friday -----
常用阻塞队列
ArrayBlockingQueue：数组结构组成的有界阻塞队列
LinkedBlockingQueue：链表结构组成的有界阻塞队列
PriorityBlockingQueue：支持优先级排序的无界阻塞队列
DelayQueue：使用优先级队列实现的误解阻塞队列
SynchronousQueue：一个不存储元素的阻塞队列
LinkedTransferQueue:由链表结构组成的无界阻塞队列
LinkedBlockingQeque：由链表结构组成的双向阻塞队列

队列操作方法：
add  不阻塞抛异常
remove

offer false
poll null 超时机制

take 空：阻塞拿元素
put	满：阻塞放元素


CAS（Compare And Swap）问题
- ABA
- 自旋消耗CPU资源
- 只能保证一个共享变量的原子操作

***
* AtomicReference

　　通过volatile和Unsafe提供的CAS函数实现原子操作。 自旋+CAS的无锁操作保证共享变量的线程安全

value是volatile类型，这保证了：当某线程修改value的值时，其他线程看到的value的值都是最新的值，即修改之后的volatile的值
通过CAS设置value。这保证了：某线程池通过CAS函数（如compareAndSet函数）设置value时，它的操作时原子性的，即线程在操作vu略时不会被中断。
但是CAS操作可能存在ABA问题。AtomicStampedReference的出现就是为了解决这问题

* AtomicStampedReference（标注被修改过几次）
构造方法中initialStamp（时间戳）用来唯一标识引用变量，在构造器内部，实例化了一个Pair对象，Pair对象记录了对象引用和时间戳信息，采用int作为时间戳，实际使用的时候，要保证时间戳唯一（一般做成自增的），如果时间戳如果重复，还会出现ABA的问题。

* AtomicStampedReference中的每一个引用变量都带上了pair.stamp这个时间戳，这样就可以解决CAS中的ABA的问题。


AtomicMarkableReference（关注有没有被修改过）
AtomicMarkableReference的唯一区别就是不再用int标识引用，而是使用boolean变量——表示引用变量是否被更改过。

[AtomicReference，AtomicStampedReference与AtomicMarkableReference的区别](https://www.cnblogs.com/xyhz0310/p/9627582.html)

[java高并发基础篇之线程执行顺序的控制](https://blog.csdn.net/qq_41071876/article/details/106010590)  
一、CountDownLatch  
二、CyclicBarrier  
三、Semaphore  
四、Exchanger  
五、Phaser

***
[java高并发基础篇之多线程Future设计模式](https://blog.csdn.net/qq_41071876/article/details/106087734)


### ----2020.5.14（庚子年四月廿二）Thursday -----
[java中isAssignableFrom()方法与instanceof关键字用法及通过反射配合注解为字段设置默认值](https://blog.csdn.net/qq_36666651/article/details/81215221)
isAssignableFrom()方法与instanceof关键字的区别总结为以下两个点：

isAssignableFrom()方法是从类继承的角度去判断，instanceof关键字是从实例继承的角度去判断。
isAssignableFrom()方法是判断是否为某个类的父类，instanceof关键字是判断是否某个类的子类。
使用方法：

父类.class.isAssignableFrom(子类.class)
子类实例 instanceof 父类类型

***



### ----2020.5.13（庚子年四月廿一）Wednesday -----
理清synchronized wait notify关系


https://www.typora.io/
markdown


hsdis
hotspot disassembler


JIT编译器

java解释执行

StampedLock


0x80中断
90H中断

cpu指令
ring0

锁重入
lock record会进入栈
为了支持继承重写




PS+P0(经历15次gc，分代年龄)
G1（5）
ZGC（不判断年龄）

(FGC)full GC

HOTSPOT

synchronized(o)
无锁  001
偏向锁101(匿名偏向：jvm虚拟机启动4s后添加状态)
自旋锁 00  轻量级锁（轻度竞争）
重量锁 10  重量级锁（重度竞争，耗时过长，wait直接启动）
GC     11


1． Little endian：将低序字节存储在起始地址（即小的字节先存放）
2． Big endian：将高序字节存储在起始地址（即大的字节先存放）



偏向锁（大多数情况）


StringBuffer
Vector


(JOL)Java Object Layout

Object o= new Object();
markword-------8byte(64bit)
klass pointer--4byte(32bit)
instance-------0byte
padding--------4byte


markword
锁
GC
hashcode(identity)

CompareAndSet

lock Atomic::cmpxhg



maven
openjdk.classlayout

ClassLayout.parseInstance(o).toPrintable();




### ----2020.5.12（庚子年四月二十）Tuesday -----
descendant	英[dɪˈsendənt]
美[dɪˈsendənt]
n.	后裔; 后代; 子孙; (由过去类似物发展来的) 派生物;

cmoveTaskToBack(true)====等价于点击HOME键

* 查看当前任务栈Task  
 adb shell dumpsys activity activities | sed -En -e '/Stack #/p' -e '/Running activities/,/Run #0/p'


android:configChanges="orientation|keyboardHidden|screenSize"

### ----2020.5.11（庚子年四月十九）Monday -----
ThreadLocal使用场景：
解决数据库连接、Session管理等
	
1.Hiberante的Session 工具类HibernateUtil
2.通过不同的线程对象设置Bean属性，保证各个线程Bean对象的独立性。

spring中使用ThreadLocal来设计TransactionSynchronizationManager类，实现了事务管理与数据访问服务的解耦，同时也保证了多线程环境下connection的线程安全问题。

***
[Android利用GradientDrawable定义动态的shape形状探索](https://blog.csdn.net/SimonHunt/article/details/72477590)  
[Android Drawable之GradientDrawable](https://www.jianshu.com/p/dbccf8dfe3ef)  

### ----2020.5.10（庚子年四月十八）Sunday -----
* ()->lambda expression
* ::----method reference

### ----2020.5.9（庚子年四月十七）Saturday -----
[全面深入地掌握NDK技术，成为下一波5G时代的浪潮儿~](https://github.com/JsonChao/Awesome-Android-NDK)  

[GitHub 热榜：文字识别神器，超轻量级中文 OCR！](https://mp.weixin.qq.com/s/RTBiM9r9MwZxwlxbhLhNEg)  
[超轻量级中文ocr，支持竖排文字识别, 支持ncnn推理 , psenet(8.5M) + crnn(6.3M) + anglenet(1.5M) 总模型仅17M](https://github.com/ouyanghuiyu/chineseocr_lite)  

### ----2020.5.8（庚子年四月十六）Friday -----
[android小知识]removeCallbacks与postDelayed的恩怨史（removeCallbacks所谓的无效, View和Handler 的postDelayed）
https://blog.csdn.net/bluewindtalker/article/details/51984300

***
[详解 Java 常用的四种锁机制优缺点](https://blog.csdn.net/valada/article/details/84540368)
（Synchronized、ReentrantLock、Semaphore、AtomicInteger）

***
AndroidManifest文件配置
android:supportsRtl
从Android 4.2开始，Android SDK支持一种从右到左（RTL，Right-to-Left）UI布局的方式，尽管这种布局方式经常被使用在诸如阿拉伯语、希伯来语等环境中，中国用户很少使用

android:allowBackup
Android 2.2中引入的系统备份功能,android:allowBackup(默认为 true )来设置应用数据是否能能够被备份或恢复
[Android之allowBackup属性](https://blog.csdn.net/mysimplelove/article/details/84073013)  


### ----2020.5.7（庚子年四月十五）Thursday -----
[Luban(鲁班)—Image compression with efficiency very close to WeChat Moments/可能是最接近微信朋友圈的图片压缩算法](https://github.com/Curzibn/Luban)
	
	//将文件路径字符串列表转化为文件列表
	Flowable.just(photos)
	.observeOn(Schedulers.io())
	.map(new Function<List<String>, List<File>>() {
	  @Override public List<File> apply(@NonNull List<String> list) throws Exception {
	    // 同步方法直接返回压缩后的文件
	    return Luban.with(MainActivity.this).load(list).get();
	  }
	})
	.observeOn(AndroidSchedulers.mainThread())
	.subscribe();

***

GIF(Graphics Interchange Format)的原义是“图像互换格式”
GIF文件的数据，是一种基于LZW算法的连续色调的无损压缩格式.

***
**睡眠1000毫秒不同写法**  
	
	android.os.SystemClock.sleep(1000);// similar to Thread.sleep(millis), but it **ignores InterruptedException**.
	
	throws InterruptedException
		java.lang.Thread.sleep(5000);
		java.util.concurrent.TimeUnit.MILLISECONDS.sleep(1000);


### ----2020.5.6（庚子年四月十四）Wednesday -----

** 子线程中启动的Activity与主线程中启动Activity有什么区别？**





jetpack +mvvm结合使用

享学课堂-薇薇:
mvvm第一节：链接: https://pan.baidu.com/s/1ELGSv3vaF5Hfm81n1ZiQmw 提取码: ftur
享学课堂-薇薇:
mvvm第二节链接：https://pan.baidu.com/s/1wreePMHn07iDy0U7fXNgHg 
提取码：cox9
mvvm第三节：链接：https://pan.baidu.com/s/1VHjzGZVqYFyPoBuq03Ojtw 
提取码：wko9
链接: https://pan.baidu.com/s/199u0sOP-6YlSjA78nZX_aA 提取码: eqx9


https://space.bilibili.com/441387550/


https://space.bilibili.com/544029825/





java.lang.instrument.Instrumentation

***
android.app.Instrumentation
Android instrumentation是Android系统里面的一套控制方法或者”钩子“

https://blog.csdn.net/a19891024/article/details/54342799

这些钩子可以在正常的生命周期（正常是由操作系统控制的)之外控制Android控件的运行，其实指的就是Instrumentation类提供的各种流程控制方法，下表展示了部分方法的对应关系

Method | Control by User(Instrumentation) | Control by OS  |
--------   | -----:   | :----:|
onCreate|callActivityOnCreate|onCreate |  
onDestroy|callActivityOnDestroy|onDestroy |   
onStart|callActivityOnStart|onStart|   


markdown快速生成

Markdown创建表格
https://www.jianshu.com/p/b0f56b7d7ee8

| 水果        | 价格    |  数量  |
| --------   | -----:   | :----: |
| 香蕉        | $1      |   5    |
| 苹果        | $1      |   6    |
| 草莓        | $1      |   7    |






### ----2020.5.5（庚子年四月十三-立夏）Tuesday -----
lateX：android展示数学公式

* 作业：利用反射、注解、动态代理实现OnClick事件的自动注入

	@Click({R.id.bottom,R.id.end})
	public void abc(View view){
			
	}

### ----2020.5.4（庚子年四月十二）Monday -----


### ----2020.5.3（庚子年四月十一）Sunday -----
RxJava

### ----2020.5.2（庚子年四月初十）Saturday -----
[ConstraintLayout](https://juejin.im/post/5d12c4146fb9a07ea33c24b7)

12:constraintTop_toTopof
7:android:layout_marginTop
6:layout_goneMarginTop

* baseline
	app:layout_constraintBaseline_toBaselineOf="@id/tvHello"

* Guideline

* 圆形定位(Added in 1.1)circle radius angle
	layout_constraintCircle : 另外一个view的id,上图的A view
	layout_constraintCircleRadius : 半径，上图的radius
	layout_constraintCircleAngle : 角度，上图angle，范围为0-360
	根据上面上个属性就可以确定B View的位置。从图也可以知道，角度以时间12点为0，顺时针方式。


**Centering positioning and bias**
ConstraintLayout居中则采用左右上下边来约束居中。

* 水平居中 layout_constraintLeft_toLeftOf & layout_constraintRight_toRightOf
* 垂直居中 layout_constraintTop_toTopOf & layout_constraintBottom_toBottomOf
* 中间居中 水平居中 & 垂直居中  
```
	<TextView
		...
		android:text="Hello"
		app:layout_constraintLeft_toLeftOf="parent"
		app:layout_constraintRight_toRightOf="parent"/>
	
```

* layout_constraintWidth="true)


* 比例约束
控件的宽高比，要求是宽或高至少一个设为0dp，然后设置属性layout_constraintDimensionRatio即可。


* Chain
	layout_constraintHorizontal_chainStyle 水平方向链式
	layout_constraintVertical_chainStyle 垂直方向链式
	

[MotionLayout：一个可以直接写动画的ConstraintLayout](https://www.jianshu.com/p/106c056772ec)  
[MotionLayout动画](https://blog.csdn.net/u014290233/article/details/94398813)
https://github.com/LGD2009/MotionLayoutExample


* Group（组）
	用来控制一组view的可见性，如果view被多个Group控制，则以最后的Group定义的可见性为主。



### ----2020.5.1（庚子年四月初九）Friday -----
极坐标定位（半径、角度）
笛卡尔坐标定位（第几行第几列)


自定义View几种方式
事件拦截/分发流程dispatchTouch
事件处理机制
滑动冲突解决方式

享学课堂
1. 获得Android VIP基础班免费学习名额
2. 600元课程优惠券
3. 价值2180元的面试专题全套课程赠送

[蒲公英API](https://www.pgyer.com/doc/view/api#paramInfo)

[钉钉开发文档](
https://ding-doc.dingtalk.com/doc#/serverapi2/qgx3dh)



https://maven.aliyun.com/mvn/view

maven{ url "https://raw.github.com/bmob/bmob-android-sdk/master"}
maven{ url "https://maven.aliyun.com/repository/google"}
maven{ url "https://maven.aliyun.com/repository/public"}
maven{ url "https://maven.aliyun.com/nexus/content/groups/public/" }
maven{ url "https://maven.aliyun.com/repository/jcenter"}
maven{ url "https://maven.aliyun.com/repository/central"}
maven{ url "https://maven.aliyun.com/repository/gradle-plugin"}

public-->central仓和jcenter仓的聚合仓	
https://maven.aliyun.com/repository/public 或 https://maven.aliyun.com/nexus/content/groups/public



### ----2020.4.30（庚子年四月初八）Thursday -----

[三大Java虚拟机(HotSpot,JRockit,IBM JVM)垃圾回收机制的比较](https://blog.csdn.net/ZYC88888/article/details/70918799?utm_source=blogxgwz4)  

**jfinal**
JAVA WEB + ORM Framework http://www.jfinal.com （作者：詹波）
https://github.com/jfinal/jfinal


[Jboot](http://jboot.io/)
一个开源的分布式、商业级微服务框架


**曾经的老框架**
AndroidAnnotation
https://github.com/androidannotations/androidannotations

**Afinal**  
Afinal是一个android的ioc，orm框架，内置了四大模块功能：FinalAcitivity,FinalBitmap,FinalDb,FinalHttp。---作者：杨福海(微信：wx198819880)

***
屏幕自动适配：修改dimension、百分比布局、autolayout


百分比布局
[Android-RatioLayout](https://github.com/mapleqin/Android-RatioLayout)  

[AndroidAutoSize](https://github.com/JessYanCoding/AndroidAutoSize)  
 A low-cost Android screen adaptation solution (今日头条屏幕适配方案终极版，一个极低成本的 Android 屏幕适配方案).

***
[ConstraintLayout,看完一篇真的就够了么？](https://juejin.im/post/5d12c4146fb9a07ea33c24b7)

***
[Android实现全部状态栏透明或者隐藏](https://www.jianshu.com/p/5d43548c05ce)  

    //获取手机状态栏高度
    public static int getStatusBarHeight(Context context) {
        Class<?> c = null;
        Object obj = null;
        Field field = null;
        int x = 0, statusBarHeight = 0;
        try {
            c = Class.forName("com.android.internal.R$dimen");
            obj = c.newInstance();
            field = c.getField("status_bar_height");
            x = Integer.parseInt(field.get(obj).toString());
            statusBarHeight = context.getResources().getDimensionPixelSize(x);
        } catch (Exception e1) {
            e1.printStackTrace();
        }
        return statusBarHeight;
    }

***
**luyten**
luyten反编译工具是一款github的开源工具，目前支持.exe、.jar和源代码下载，还是充分的考虑到windows用户了，jd显示INTERNAL ERROR的class文件笔者用这个可以打开，并且设置比jd丰富。

[Java电子书库](https://github.com/singgel/JAVA)  

***

**Java四大名著**
Think in java, Effective Java , Core Java(Volume I--Fundamentals & Volume II--Advanced Features) , java编程语言----JamesGosling

* Java编程语言（第三版)---Java四大名著----James Gosling(Java之父)  
* Java编程思想（第4版)----Java四大名著------------Bruce Eckel  
* JAVA 2核心技术 卷I：基础知识（原书第8版）---Java四大名著-----Cay Horstmann   
	JAVA 2核心技术 卷II：高级特性（原书第8版)----Java四大名著-----Cay Horstmann  
* Effective Java中文版------Java四大名著--------Joshua Bloch

[Java世界里的四大名著(Java程序员必看书籍)](https://blog.csdn.net/qq_38584262/article/details/83793854)  

***
* 所有界面都显示悬浮球
	一个要悬浮窗，一个不用悬浮窗（只能在应用内）
	https://www.jianshu.com/p/7d1a7c82094a  
	https://github.com/feiyuu/FloatingView 




### ----2020.4.29（庚子年四月初七）Wednesday -----
[Android 后台运行白名单，优雅实现保活](https://www.cnblogs.com/Android-Alvin/p/12465949.html?tdsourcetag=s_pctim_aiomsg)  
* 保活"黑科技":1像素Activity，播放无声音频，双进程互相守护

[优雅保活方案，原来Android还可以这样保活！](https://www.jianshu.com/p/8736f4fadb66)  
提高app的保活可能性，项目中使用1px像素Activity ，前台服务，播放无声音乐，Job Service等方法。
手机设置：进程加锁，自启动，允许后台运行，部分机型有解冻app设置。

[2017-2020历年字节跳动Android面试真题解析（累计下载1082万次，持续更新中）](https://www.cnblogs.com/Android-Alvin/p/12448764.html)  

https://github.com/LingCoder/OnJava8
第五版别人的中文业余翻译

[《On Java 8》中文版]https://lingcoder.github.io/OnJava8/#/sidebar

[《Java编程思想》中文第5版](https://lingcoder.github.io/OnJava8/)



### ----2020.4.28（庚子年四月初六）Tuesday -----
Annotation Processing Tool (APT)

ConstraintLayout

Retrofit
动态代理+注解+反射


### ----2020.4.27（庚子年四月初五）Monday -----
**反射**  

java.lang.reflect   
接口 Type  
所有已知子接口：   
GenericArrayType, ParameterizedType, TypeVariable<D>, WildcardType   
所有已知实现类： 
Class 

public interface TypeType 是 Java 编程语言中所有类型的公共高级接口。它们包括原始类型、参数化类型、数组类型、类型变量和基本类型。 

从以下版本开始： 
1.5 

***
[注解作用目标限定和保留策略](https://blog.csdn.net/u011541946/article/details/100057926)  
**注解作用目标**
java.lang.annotation 
注解类型 Target
***
@Documented  
@Retention(value=RUNTIME)  
@Target(value=ANNOTATION_TYPE)  
public @interface Target  

从以下版本开始： 
1.5 

	java.lang.annotation 
	枚举 ElementType
	java.lang.Object
	  继承者 java.lang.Enum<ElementType>
		  继承者 java.lang.annotation.ElementType
	所有已实现的接口： Serializable, Comparable<ElementType> 
	
	ANNOTATION_TYPE	注解类型声明 
	CONSTRUCTOR 构造方法声明 
	FIELD 字段声明（包括枚举常量） 
	LOCAL_VARIABLE 局部变量声明 
	METHOD 方法声明 
	PACKAGE 包声明 
	PARAMETER 参数声明 
	TYPE 类、接口（包括注解类型）或枚举声明 



**注解保留策略**
-
java.lang.annotation 
注解类型 Retention

@Documented  
@Retention(value=RUNTIME)  
@Target(value=ANNOTATION_TYPE)  
public @interface Retention指示注解类型的注解要保留多久。如果注解类型声明中不存在 Retention 注解，则保留策略默认为 RetentionPolicy.CLASS。 

只有元注解类型直接用于注解时，Target 元注解才有效。如果元注解类型用作另一种注解类型的成员，则无效。 

从以下版本开始： 
1.5 



* 源代码文件注解（SOURCE）：  
	注解只保留在源代码文件，当编译时，会被忽略，在字节码中是不会存在的。所以，反编译别人的源码，是不会存在注解的。
* 字节码文件注解（CLASS）：  
	这种注解，在源代码中存在，然后编译时会把注解信息放在class文件中，但JVM在加载类的时候会忽略注解。
* JVM中注解（RUNTIME）：  
	在源码文件中存在，在JVM加载的时候会把注解加载到JVM内存，这个是唯一可反射注解。

	java.lang.annotation  
	枚举 RetentionPolicy  
	java.lang.Object  
	  继承者 java.lang.Enum<RetentionPolicy>  
		  继承者 java.lang.annotation.RetentionPolicy  
	所有已实现的接口： 
	Serializable, Comparable<RetentionPolicy>   
	public enum RetentionPolicy extends Enum<RetentionPolicy>注解保留策略。此枚举类型的常量描述保留注解的不同策略。它们与 Retention 元注解类型一起使用，以指定保留多长的注解。 

	从以下版本开始： 
	1.5 

	枚举常量摘要   
	SOURCE 编译器要丢弃的注解。   
	CLASS 编译器将把注解记录在类文件中，但在运行时 VM 不需要保留注解。   
	RUNTIME 编译器将把注解记录在类文件中，在运行时 VM 将保留注解，因此可以反射性地读取。  

***



**java四种引用**
```
java.lang.ref 
类 ReferenceQueue<T>
java.lang.Object
  继承者 java.lang.ref.ReferenceQueue<T>

------------------
public class ReferenceQueue<T> extends Object  
引用队列，在检测到适当的可到达性更改后，垃圾回收器将已注册的引用对象添加到该队列中。 



强、
软：SoftReference
	java.lang.Object
  继承者 java.lang.ref.Reference<T>
      继承者 java.lang.ref.SoftReference<T>
	构造方法摘要 
	SoftReference(T referent) 
          创建引用给定对象的新的软引用。 
	SoftReference(T referent, ReferenceQueue<? super T> q) 
          创建一个引用给定对象的新的软引用，并向给定队列注册该引用。 

	//软可到达对象的所有软引用都要保证在虚拟机抛出 OutOfMemoryError 之前已经被清除。然而，虚拟机实现不鼓励清除最近访问或使用过的软引用。 
	//此类的直接实例可用于实现简单缓存


弱：WeakReference
java.lang.Object
  继承者 java.lang.ref.Reference<T>
      继承者 java.lang.ref.WeakReference<T>
	构造方法摘要 
	WeakReference(T referent) 
          创建引用给定对象的新的弱引用。 
	WeakReference(T referent, ReferenceQueue<? super T> q) 
          创建引用给定对象的新的弱引用，并向给定队列注册该引用。 
	//弱引用最常用于实现规范化的映射。 -->ThreadLocal


虚：PhantomReference
java.lang.Object
  继承者 java.lang.ref.Reference<T>
      继承者 java.lang.ref.PhantomReference<T>
	
	构造方法摘要
	PhantomReference(T referent, ReferenceQueue<? super T> q) 
	创建一个引用给定对象的新的虚引用，并向给定队列注册它。
```

```
正向代理
[正向代理与反向代理的区别](https://www.jianshu.com/p/208c02c9dd1d)  
[正向代理和反向代理的区别]（https://www.tuicool.com/articles/M7bAnqy)  
正向代理（代理封装客户端）应用场景：Squid科学上网  
反向代理（代理封装服务端）应用场景：Nginx
* 负载均衡
* 保护和隐藏原始资源服务器
* 加密和SSL加速
* 缓存静态内容
* 压缩
* 减速上传
* 安全
* 外网发布
```

***
要价12580大洋的课程
[网易工程师带你突破Android技术瓶颈](https://mooc.study.163.com/smartSpec/detail/1202810601.htm)
-  UI/NDK开发 · 性能优化 · 架构设计 · Flutter开发
***



### ----2020.4.26（庚子年四月初四）Sunday -----
> java中**协变**跟**逆变**是对泛型类的继承关系的表述.
> Number为Integer的父类
> List<Number> 和List<Integer> 之间是没有继承关系的
> **协变**  协变主要是用在函数的返回值上
>  List<Integer> 是 List<? extends Number> 的子类型
>  Crate<Orange> 是 Crate<? extends Fruit> 的子类型
> ***
> **逆变** 逆变用在函数参数上
> List<Number> 是 List<? super Integer> 的子类型
> Crate<Fruit> 是 Crate<? super Orange> 的子类型
> ***
> [Java和Kotlin中泛型的协变、逆变和不变](https://www.jianshu.com/p/0c2948f7e656)  
> ``` 
> type variance（型变）  
> Type variance refers to the techniques by which we can allow, or not allow, subtyping in our parameterized types.
> ```
> invariance（不型变）：也就是说，Crate<Orange> 和 Crate<Fruit> 之间没有关系。  
> covariance（协变）：也就是说，Crate<Orange> 是 Crate<? extends Fruit> 的子类型。  
> contravariance（逆变）：也就是说，Crate<Fruit> 是 Crate<? super Orange> 的子类型。  
> 子类（subclass） 和 子类型（subtype）不是一个概念    
> 子类一定是子类型，子类型不一定是子类，例如，Crate<Orange> 是 Crate<? extends Fruit> 的子类型，但是Crate<Orange> 并不是 Crate<? extends Fruit> 的子类。  




### ----2020.4.25（庚子年四月初三）Saturday -----
Thread中断
* static	boolean interrupted()	测试当前线程是否已经中断。  
public static boolean interrupted()测试当前线程是否已经中断。线程的中断状态 由该方法清除。换句话说，如果连续两次调用该方法，则第二次调用将返回 false（在第一次调用已清除了其中断状态之后，且第二次调用检验完中断状态前，当前线程再次中断的情况除外）。 
线程中断被忽略，因为在中断时不处于活动状态的线程将由此返回 false 的方法反映出来。 
	返回：
	如果当前线程已经中断，则返回 true；否则返回 false。

* boolean isInterrupted()	测试线程是否已经中断。   
	public boolean isInterrupted()测试线程是否已经中断。线程的中断状态 不受该方法的影响。 
线程中断被忽略，因为在中断时不处于活动状态的线程将由此返回 false 的方法反映出来。 
	返回：
	如果该线程已经中断，则返回 true；否则返回 false。	



### ----2020.4.24（庚子年四月初二）Friday -----
并行(同一时间)
并发（指定时间段范围）
Callable、FutureTask

### ----2020.4.23（庚子年四月初一）Thursday -----
IntelliJ IDEA 插件 ASM Bytecode Viewer插件
ASMPlugin:Bytecode ASMified Groovified

泛型
不能创建泛型数组

> [数组是协变的，具体化的](https://blog.csdn.net/zjq2008wd/article/details/8788310)  
> 示例：Fruit[] apples=new Apple[size];


泛型+协变=坑

CAP#1

通配符就是解决泛型不能 协变和逆变的


Box<?> 不能存也不能取,进行安全检查

Box<? extends T> 可看作只取（读取)  
Box<? super T> 主要用于存（写入)  


**泛型方法**
* 带有一个或多个类型参数的方法
* 方法参数可以包含泛型类型，方法也可以包含泛型返回类型。
* 泛型方法可以定义在普通类中，也可以定义在泛型类中。
* 只有在方法返回值之前，方法修饰符之后存在泛型参数列，这样的方法才是泛型方法。这则条件隐含着该方法要么入参包含泛型类型，要么返回值包含泛型类型。
***


##java进阶
	JVM、多线程、设计模式、Redis、ZK、MySQL调优
	算法与数据结构
	Netty（网络）



《java多线程编程实战指南》--黄文海

先栈后大再小堆，大是老人好GC



对象内存存储布局
jol(java object layout)

[JOL：查看Java 对象布局、大小工具](https://www.iteye.com/blog/shihlei-2407693)  

[Object obj = new Object()在内存中占用多少字节？](https://blog.csdn.net/linysuccess/article/details/105655614)  
64位虚拟机，开启压缩，不开启压缩都是**16byte**，坑：obj在32G内存以上会膨胀为8byte  
一个Object对象占用16个字节，那这个16个字节中分别存放的是什么内容呢？  

前面8个字节是对象头，也叫markword，记录对象被上锁的各种状态（锁升级）和垃圾回收相关信息等。  
接下来4个字节（4G堆内存以下；或者32G以内，并且开启了ClassPointer指针压缩，否则是8个字节）是一个指向对象所属Class对象的指针。  
接下来4个字节是为了8字节对齐而填充的padding。  



```
markword 		8byte  
class pointer		4byte  
instance data		0byte  
padding			4byte  
```



对象头markword klasspointer包含什么内容？（hashcode gc 锁）

cms年龄是6

biased lock偏向锁
```
####对象怎么定位？
* 句柄方式(间接定位，句柄方式GC回收比较稳定)
实例数据指针 m = 0
类型数据指针 方法区 T.class

* 直接指针



```
分配内存 调用构造 返回指针
TLAB(Thread Local Allocation Buffer)

***

java -X
java -XX
java -XX:+PrintCommandLineFlags -version

javac
javap -c

//编译成 class 文件
javac Test.java 

//反汇编 class 文件
javap -V Test.class

> IDEA 插件  
	1. jclasslib Bytecode viewer  
	2. ASM Bytecode Viewer  


​	
***
HashMap优化：避免扩容  
加载因子  
阈值0.75  
扩容：达到阈值=加载因子x默认大小  
rehash  


> 设计模式-代理模式
> * 普通代理(静态代理)
> * [虚拟代理(可类比为：代理模式+懒汉模式，需要多处判空)](https://www.cnblogs.com/noKing/p/9062329.html)  
> * 强制代理  
> * 动态代理  
> [Android设计模式之代理模式 Proxy](https://blog.csdn.net/l2show/article/details/46992495)

***
> 工具  
[英语词源](https://www.etymonline.com/)  
[词根词源字典](http://etymon.cn/index.html)  
[汉典](https://www.zdic.net/)  
[IntelliJ IDEA官方文档 W3Cschol](https://www.w3cschool.cn/intellij_idea_doc/)  
[JAVA SE6 API](https://docs.oracle.com/javase/6/docs/api/)  
[JAVA SE7 API](https://docs.oracle.com/javase/7/docs/api/)  
[JAVA SE8 API](https://docs.oracle.com/javase/8/docs/api/)  
[JAVA SE10 API](https://docs.oracle.com/javase/10/docs/api/)  
[JAVA SE14 API](https://docs.oracle.com/en/java/javase/14/docs/api/index.html)  
[java8 language specification](https://docs.oracle.com/javase/specs/jls/se8/html/index.html)  


[java6 api在线中文](https://tool.oschina.net/apidocs/apidoc?api=jdk-zh)
[java8 api在线中文](http://www.matools.com/api/java8)  
[open jdk](http://openjdk.java.net/)  
[jdk14 download](http://jdk.java.net/14/)


[jdk1.8 API中文翻译](https://gitee.com/aLiez/java8-zh)

***
* GitHub:Android选择器（时间、省市区三级联动  
[时间选择器、省市区三级联动](https://github.com/Bigkoo/Android-PickerView)

https://github.com/saiwu-bigkoo?tab=repositories
***
Activity>PhoneWindow>DecorView>(TitleView|ContentView)

[Android窗口机制（一）认识Android的窗口结构](https://blog.csdn.net/HoHohong/article/details/54412449)  
[Android窗口机制（二）Window，PhoneWindow，DecorView，setContentView源码理解](https://blog.csdn.net/HoHohong/article/details/54412464)
***


java.lang.Object
	java.text.Format
* All Implemented Interfaces:
	Serializable, Cloneable
* Direct Known Subclasses:
	DateFormat, MessageFormat, **NumberFormat**
	

NumberFormat (Java Platform SE 7 )
java.lang.Object  
	java.text.Format  
		java.text.NumberFormat 
		
* All Implemented Interfaces:  
	Serializable, Cloneable
* Direct Known Subclasses:
	ChoiceFormat, DecimalFormat
	
```
                 |-- java.text.MessageFormat
java.text.Format—|
		 |			   |--java.text.ChoiceFormat
		 |--java.text.NumberFormat—|
		 |			   |--java.text.DecimalFormat
		 |
		 |--java.text.DateFormat—java.text.SimpleDateFormat
```

java.text.NumberFormat类有三个方法可以产生下列数据的标准格式化器：  
创建格式化器(默认地区Local格式)：  
NumberFormat.getNumberInstance();//数字格式化器  
NumberFormat.getCurrencyInstance();//货币格式化器  
NumberFormat.getPercentInstance();//百分数格式化器  

**整数或小数部分所显示的最少和最多位数**  
设定整数或小数部分所显示的最少和最多位数，可以使用NumberFormat类的方法：  
setMinimumIntegerDigits(int)//设定整数最小位数  
setMinimumFractionDigits(int)//设定小数最少位数  
setMaximumIntegerDigits(int)//设定整数最多位数  
setMaximumFractionDigits(int)//设定小数最多位数  


* 设定小数部分的最多位很有用处。
	如果小数部分丢失的第一位数字大于等于5，那么显示的最后一位会增1（四舍五入）。  
	如果要显示尾随的零，可以把小数部分的最少位等于最多位。  
	如果不想显示，可以把小数部分的最少位设定为0或不设定。  

* 指定最多位整数相当危险，显示值将会被截断，产生一个错误的值。

> 原文链接：  
[java.text.NumberFormat使用](https://blog.csdn.net/junshuaizhang/article/details/8559708)

***
### ----2020.4.22（庚子年三月三十）Wednesday -----
六大原则
单一职责原则（SRP：Single Pesponsibility Principle）
开放封闭原则（OCP：Open Closed Principle）--Open（Open for extendtion）开放支持扩展，Close（Closed for modification）
里氏替换原则（LSP：Liskov Substitution Principl）
依赖倒置原则（DIP：Dependence Inversion Principle）
接口隔离原则（ISP：Interface Segregation Principle）
最少知识原则（LKP：Least Knowledge Principle）又叫迪米特原则（Law of Demeter）,简单说成：talk only to your immediate friends


[okhttp官网](https://square.github.io/okhttp/)

***
kHttp3的最底层是Socket，而不是URLConnection，它通过Platform的Class.forName()反射获得当前Runtime使用的socket库，调用栈如下

okhttp//实现HTTP协议  
==>framwork//JRE，实现JDK中Socket封装  
    ==>jvm//JDK的实现，本质对libc标准库的native封装  
        ==>bionic//android下的libc标准库  
            ==>systemcall//用户态切换入内核  
                ==>kernel//实现下协议栈(L4,L3)与网络驱动(一般是L2,L1)  

注：需求决定，Android版本4.4.4 okhttp 3.2.0

原文链接：https://blog.csdn.net/hello2mao/article/details/53159151

***
@SuppressWarnings
压制警告

* android.widget.FrameLayout  
public class FrameLayout extends ViewGroup

***
设计模式:Composite--组合模式-树形结构

***
> 工具：
* [知识圈助手](https://intools.cn/PCoverview)
* PC QQ 滑动鼠标截长图：Ctrl+Alt+A



[ViewPager不能高度自适应？height=wrap_content 无效解决办法](https://www.cnblogs.com/zhujiabin/p/4818551.html) -->重写onMeasure

[Android为什么在RecyclerView中使用executePendingBindings](http://www.6tie.net/p/1272494.html)

[Android Why use ExecutePendingBindings](https://stackoverflow.com/questions/52996894/android-why-use-executependingbindings)


MD(Material Design)


* [BRVAH](https://github.com/CymChad/BaseRecyclerViewAdapterHelper)
> 强大而灵活的RecyclerView Adapter http://www.recyclerview.org/

***
凡使用Adapter选项高度设定：包一层布局

 public FrameLayout(@NonNull Context context, @Nullable AttributeSet attrs,
            @AttrRes int defStyleAttr, @StyleRes int defStyleRes) 
			
***
public View inflate(XmlPullParser parser, @Nullable ViewGroup root, boolean attachToRoot)
常用方法：View inflate(int resource, ViewGroup root)

setContentView vs LayoutInflater.inflate  
* 联系：
	目的都是把xml表述的layout转化为View对象   
	 Activity.setContentView底层PhoneWindow.setContentView最终调用的也是mLayoutInflater.inflate
	 //将要加载的资源添加到mContentParent上
     mLayoutInflater.inflate(layoutResID, mContentParent);
	
	 new com.android.internal.policy.PhoneWindow(this, window, activityConfigCallback);
* 区别：
	1. setContentView()一旦调用, layout就会立刻显示UI；  
	inflate只会把Layout形成一个以view类实现成的对象，可通过调用setContentView(view)显示出来  
	2. 在activity中通过setContentView()将界面显示出来，在非activity中对控件布局设置操作需要用LayoutInflater动态加载
***
* LiveData=LifecycleObserver+DataObserver

***
**LoadSir**是一个高效易用，低碳环保，扩展性良好的加载反馈页管理框架，在加载网络或其他数据时候，根据需求切换状态页面，可添加自定义状态页面，如加载中，加载失败，无数据，网络超时，占位图，登录失效等常用页面。可配合网络加载框架，结合返回状态码，错误码，数据进行状态页自动切换，封装使用效果更佳。
A lightweight, good expandability Android library used for displaying different pages like loading, error, empty, timeout or even your custom page when you load a page.(优雅地处理加载中，重试，无数据等)
[LoadSir Github传送门](https://github.com/KingJA/LoadSir)

***
异步：线程池、多线程、链式调度、设计模式

### ----2020.4.21（庚子年三月廿九）Tuesday -----
> 后端：分库分表（水平分表策略：区间、取模）
***
> 为什么使用泛型？  
	1. 编译时类型检查  
	2. 消除类型强制转化
	3. 实现通用算法-->代码复用

***
** 自定义View**

** 描述MeasureSpec的原理**

MeasureSpec用一个32位的int来表示一个View测量规格  
	前2位表示测量规格模式(mode)  
	后30位表示测量规格尺寸大小(size)
	
```
子View的大小及测量模式由父View的测量模式和子View的LayoutParams决定
LayoutParams取值有三种：dp（精确值）,match_parent,wrap_content 
根据父view的三种测量模式和子View的三种LayoutParams会得出九种结果
```


	private static final int MODE_SHIFT = 30;
	private static final int MODE_MASK  = 0x3 << MODE_SHIFT;

1. 未指定模式（android.view.View.MeasureSpec#UNSPECIFIED）  
当前父View未对子View加任何限制，可以随便用空间，不受限制。
	
		/**
		 * Measure specification mode: The parent has not imposed any constraint
		 * on the child. It can be whatever size it wants.
		 * 最高两位是00的时候表示"未指定模式"。即MeasureSpec.UNSPECIFIED  
		 */
		public static final int UNSPECIFIED = 0 << MODE_SHIFT;//00
	
2. 精确模式（android.view.View.MeasureSpec#EXACTLY）  
父View对子View尺寸有精确限定。无论子View想要多大尺寸，但都已被已父View限定了范围。
	
		/**
		 * Measure specification mode: The parent has determined an exact size
		 * for the child. The child is going to be given those bounds regardless
		 * of how big it wants to be.
		 *最高两位是01的时候表示"'精确模式"。即MeasureSpec.EXACTLY
		 */
		public static final int EXACTLY     = 1 << MODE_SHIFT;//01
	
	
	
3. 最大模式（android.view.View.MeasureSpec#AT_MOST）  
子View想要多大就多大,当然子View也可以用很小的尺寸  
	
		 /**
		 * Measure specification mode: The child can be as large as it wants up
		 * to the specified size.
		 *最高两位是10的时候表示"最大模式"。即MeasureSpec.AT_MOST
		 */
		public static final int AT_MOST     = 2 << MODE_SHIFT;//10

参考：  
[MeasureSpec中三种模式：UNSPECIFIED，AT_MOST，EXACTLY](https://blog.csdn.net/mp624183768/article/details/79622527)

***
parentMeasureSpec和childMeasureSpec为什么会存在这样的转换关系？我是这样理解的：

1. 当子view指定精确的大小时，无论父容器的测量模式是什么，父容器都会依据子view所要求的dimension来确定子view的大小，即子view的模式是EXACTLY。
2. 当父容器为精确模式时,父容器的大小就确定了。如果子view的属性是match_parent，子view填满父容器，子view的大小就等于父容器的大小，那么子view的模式就是EXACTLY；如果子view的属性为wrap_content，那么子view的大小是不确定的，但是必须小于父容器的size，所以子view的MeasureSpec为AT_MOST+size。
3. 当父器为AT_MOST最大模式时，这是时父容器的大小不确定，但是不能大于size。此时不论子view的属性是match_parent还是wrap_content，模式都是最大模式，并且小于size。
4. 当父器为UNSPECIFIED未知模式时，此时无论子view的dimension为多大都是可以的，因为这个模式下父容器不限制子view的大小，要多大有多大。

原文：[View的三种测量模式的理解](https://blog.csdn.net/yangtssj/article/details/71634229)




**自定义View，为什么要进行measure？ **
通过measure可以测量出实际宽高尺寸，

***
**OOM_ADJ (Out of Memory Adjustment)** 
是android系统在内存不足情况下进行内存调整的重要参数，OOM_ADJ 取值：
[Android的OOM_ADJ](https://www.jianshu.com/p/8897b7e47466)


### ----2020.4.20（庚子年三月廿八）Monday -----

Links:
> **JOL** (Java Object Layout) is the tiny toolbox to analyze object layout schemes in JVMs.  
> [JOL](http://openjdk.java.net/projects/code-tools/jol/)



> 自定义view事件分发  
> window->decorView->ViewGroup->View.  
> 3层，简化就是：Activity的分发， ViewGroup的事件分发，View的事件分发  






### ----2020.4.19（庚子年三月廿七）Sunday -----
> **内存泄漏**  
包含Context的单例(Context使用Application)

***

> say byebye to findViewById-----ViewBinding 
[Butterknife的github主页](https://github.com/JakeWharton/butterknife)  
http://jakewharton.github.io/butterknife/

Attention: This tool is now deprecated. Please switch to view binding.

***

> Lifecycle  

	public class ComponentActivity extends androidx.core.app.ComponentActivity implements
	    LifecycleOwner,
	    ViewModelStoreOwner,
	    SavedStateRegistryOwner,
	    OnBackPressedDispatcherOwner {
***


	public class ComponentActivity extends Activity implements
			LifecycleOwner,
			KeyEventDispatcher.Component 

***
	package androidx.lifecycle;
	/**
	 * Marks a class as a LifecycleObserver. It does not have any methods, instead, relies on
	 * {@link OnLifecycleEvent} annotated methods.
	 * <p>
	 * @see Lifecycle Lifecycle - for samples and usage patterns.
	 */
	@SuppressWarnings("WeakerAccess")
	public interface LifecycleObserver {
	
	}

***
泛型PECS（Producer Extends<只读> Comsumer Super)  
[Java 泛型 <? super T> 中 super 怎么 理解？与 extends 有何不同？](https://www.zhihu.com/question/20400700)  

[《effective java》里，Joshua Bloch提出的PECS原则](http://stackoverflow.com/questions/2723397/what-is-pecs-producer-extends-consumer-super)


https://docs.oracle.com/javase/tutorial/java/generics/subtyping.html


**Get and Put Principle**

Naftalin与Wadler合著的《Java Generics and Collections 》阐述如下：

The Get and Put Principle: 
use an extends wildcard when you only get values out of a structure, 
use a super wildcard when you only put values into a structure, 
and don’t use a wildcard when you both get and put.

PECS表示producer-extends，consumer-super

上界通配符：只能读，不能写，适合频繁往外面读取内容的场景。
下界通配符：不影响写，但往外取只能放在Object对象里，适合经常往里面插入数据的场景。
***

> 软技能：拒绝的艺术

### ----2020.4.18（庚子年三月廿六）Saturday -----
**一个线程对象只能调用一次start方法.**  
从new到等待运行是单行道,所以如果你对一个已经启动的线程对象再调用一次start方法的话,会产生**IllegalThreadStateException**异常

***
[Java并发编程：Callable、Future和FutureTask](https://www.cnblogs.com/dolphin0520/p/3949310.html)  

** Future提供了三种功能：  **
　　1）判断任务是否完成；  
　　2）能够中断任务；  
　　3）能够获取任务执行结果。  

* FutureTask是Future接口的常用实现类

		public abstract class ForkJoinTask<V> implements Future<V>, Serializable 

```
JDK1.8 API Future接口
所有已知实现类： 
CompletableFuture ， CountedCompleter ， ForkJoinTask ， 
FutureTask ，RecursiveAction ， RecursiveTask ， SwingWorker
```

**Future接口的实现类**

|CompletableFuture  | CountedCompleter | ForkJoinTask |
| --- | --- | --- |
| FutureTask | RecursiveAction | RecursiveTask | SwingWorker |

* FutureTask类实现了RunnableFuture接口  

		public class FutureTask<V> implements RunnableFuture<V>

* RunnableFuture接口的实现  

		public interface RunnableFuture<V> extends Runnable, Future<V> {
			void run();
		}
	
***

KeyWord：**ColorMatrix**  
[Android改变图像的饱和度、亮度和对比度](https://blog.csdn.net/sxwyf248/article/details/7019731)

[颜色矩阵-滤镜ColorMatrix](https://www.cnblogs.com/baiqiantao/p/5491800.html)

** 色彩的三要素**
1. 色相。色相通俗的说就是“颜色”，色相的改变就是颜色的改变，色相的调节伴随着红橙黄绿蓝紫的变化。
2. 亮度。明度通俗的说就是“光照度”，明度的改变就是光照在物体上带来的改变，明度的调节伴随着越高，光越强，越泛白（就像过曝一样，往白色上偏离）；越低，光越弱，越往黑里偏
3. 饱和度。饱和度通俗的说就是“色彩的纯度”，饱和度的改变会影响颜色的鲜艳程度，以红色为例子，越高，越接近红色，越低则越接近灰色（黑白）



### ----2020.4.17（庚子年三月廿五）Friday -----




### ----2020.4.16（庚子年三月廿四）Thursday -----

 [马士兵教育直播列表](https://s1.mashibing.com/selectuser)
 [马士兵教育菜鸟预习](http://mashibing.com/html/bird.html)
 [马士兵教育vip资料](http://www.mashibing.com/vip.html)
 [马士兵教育github仓库](https://www.github.com/bjmashibing)



[《深度探索Gradle自动化构建技术（二、Groovy 筑基篇）》](https://juejin.im/post/5e97ac34f265da47aa3f6dca)

***
[SurfaceView用法](https://www.jianshu.com/p/a40c84580952)  
View是通过刷新来重绘视图，系统通过发出VSSYNC信号来进行屏幕的重绘，刷新的时间间隔是16ms,
如果我们可以在**16ms**以内将绘制工作完成，则没有任何问题。
如果我们绘制过程逻辑很复杂，并且我们的界面更新还非常频繁，这时候就会造成界面的卡顿，影响用户体验，
为此Android提供了SurfaceView来解决这一问题。  
SurfaceView拥有独立的绘图表面，因此SurfaceView的UI就可以在一个独立的线程中进行绘制。  
由于不会占用主线程资源，SurfaceView 一方面可以实现复杂而高效的UI，另一方面又不会导致用户输入得不到及时响应。
***

** 组件化方案**

* CC:ComponentCaller、
* ARouter、
* DDComponent/JIMU
* AppJoint（面向接口编程）

***

> [模拟API返回数据](https://www.easy-mock.com/)

***
>[单链表反转](https://blog.csdn.net/zxm317122667/article/details/84282723)



** ANR**

在Android里, App的响应能力是由Activity Manager和Window Manager系统服务来监控的. 通常在如下三种情况下会弹出ANR对话框:

1.  Activity 位于前台时:**5s**内无法响应用户输入事件(例如键盘输入, 触摸屏幕等)
2. BroadcastReceiver在**10s**内无法结束
3. ServiceTimeout(**20s**) --小概率类型，Service在特定的时间内无法处理完成

造成以上两种情况的首要原因就是在主线程(UI线程)里面做了太多的阻塞耗时操作, 例如文件读写, 数据库读写, 网络查询等.

链接：https://www.jianshu.com/p/4eabede8c8af

> Links: [ANR谷歌官方定义](https://developer.android.google.cn/topic/performance/vitals/anr?hl=zh_cn)
***


https://class.imooc.com/sale/newandroid?mc_marking=f322d9d94ed01283bfdc19694f44e877&mc_channel=bdazrmjt


### ----2020.4.15（庚子年三月廿三）Wednesday -----
AAR（Android Archive）
JAR（Java Archive）

```
[view，canvas，surface之间的关系](https://blog.csdn.net/daojin505/article/details/76814844)  
Views are not attached to the Canvas nor the Surface.   
The window is tied to a Surface and the ViewRoot asks the Surface for a Canvas that is then used by the Views to draw onto.

ViewRootImpl.performTraversals()  
* 1、private void performMeasure(int childWidthMeasureSpec, int childHeightMeasureSpec)  
* 2、private void performLayout(WindowManager.LayoutParams lp, int desiredWindowWidth, int desiredWindowHeight)  
* 3、private void performDraw()  
```

> Android开发方向：  
> 1. Android APP
> 2. Android后台(Java后台)
> 3. 系统级开发
> 4. Android驱动开发(嵌入式串口编程)



串口通信 用serialport:

串口和tcp差不多，一个输入流一个输出流，来一个线程读 一个线程队列写，然后就是定协议的事情了

ZLL:
图像 音频的基础和编码，ffmpeg使用


参考源码
exoplayer
ijkplayer




### ----2020.4.14（庚子年三月廿二）Tuesday -----
**vi操作**  
ESC+O	换行  
u		撤销上一步的操作  
Ctrl+r	恢复上一步被撤销的操作  


**度量单位含义**  
`dip (dp)`  
device independent pixels（设备独立像素）。  
不同设备有不同的显示效果，这个和设备硬件有关，一般我们为了支持WVGA，HVGA和QVGA推荐使用这个，不依赖像素。  
`px`  
pixels（像素）不同设备显示效果相同。  
`sp`  
scaled pixels（放大像素）主要用于字体显示（best for textsize）。  
`in`  
英寸，长度单位。  
`pt`  
point，是一个标准长度单位，1pt = 1/72英寸，用于印刷业。  

[原文链接]：https://blog.csdn.net/zinss26914/java/article/details/43732467


### ----2020.4.13（庚子年三月廿一）Monday -----
TraceView：Android平台配备的性能分析工具
使用：通过Android studio自带的traceview查看（Android profiler）



**android通过反射获取状态栏的高度**

    /**
     * 获取状态栏高度
     * @param activity
     * @return
     */
    public int getStatusHeight(android.app.Activity activity) {
        int statusHeight = 0;
        android.graphics.Rect rect = new android.graphics.Rect();
        activity.getWindow().getDecorView().getWindowVisibleDisplayFrame(rect);
        statusHeight = rect.top;
        if (0 == statusHeight) {
            Class<?> localClass;
            try {
                localClass = Class.forName("com.android.internal.R$dimen");
                Object object = localClass.newInstance();
                int height = Integer.parseInt(localClass
                        .getField("status_bar_height").get(object)
                        .toString());
                statusHeight = activity.getResources()
                        .getDimensionPixelSize(height);
            } catch (Exception e) {
                e.printStackTrace();
            }
        }
        return statusHeight;
    }
    
    //通过反射获取状态栏高度
    private void getStatusBarHeight(Context context){
        int statusBarHeight=0;
        try {
            Class clazz=Class.forName("com.android.internal.R$dimen");
            Object object=clazz.newInstance();
            java.lang.reflect.Field field=clazz.getField("status_bar_height");
            //反射出该对象中status_bar_height字段所对应的在R文件的id值
            //该id值由系统工具自动生成,文档描述如下:
            //The desired resource identifier, as generated by the aapt tool.
            int id = Integer.parseInt(field.get(object).toString());
            System.out.println("id="+id);
            //依据id值获取到状态栏的高度,单位为像素
            statusBarHeight = context.getResources().getDimensionPixelSize(id);
            System.out.println("statusBarHeight="+statusBarHeight+"pixel");
        } catch (Exception e) {
            // TODO: handle exception
        }
    }





### ----2020.4.12（庚子年三月二十）Sunday -----  
80中断



### ----2020.4.11（庚子年三月十九）Saturday -----  
CLion
CLion: A Cross-Platform IDE for C and C++ by JetBrains



### ----2020.4.10（庚子年三月十八）Friday -----

SQLiteStudio：
简单、强大的sqlite数据库调试工具  
https://github.com/pawelsalawa/sqlitestudio  
使用方法：
* 1、获得jar包：SQLiteStudioRemote.jar
* 2、将SQLiteStudioRemote.jar加入Android项目
* 3、在application中添加代码：  
`SQLiteStudioService.instance().start(this)`


自定义控件 - 流式布局（FlowLayout） 
https://www.jianshu.com/p/41e63a9e10bb


MVPArms:可配置化的 Android MVP 快速集成框架   
https://github.com/JessYanCoding/MVPArms

ArmsComponent:MVPArms 官方快速组件化方案  
https://github.com/JessYanCoding/ArmsComponent


ContentProvider主要用于数据管理和数据共享的功能，主要优势为数据共享  
适用于经常需要给其他App提供数据的场景。  
如系统内置应用：联系人，日历和短信，就比较适合使用ContentProvider



ConstraintLayout


### ----2020.4.9（庚子年三月十七）Thursday -----

**自定义View**
	ViewRootImpl.performTransversal

##前端-JetPack系列
androidx.work.WorkManager
调度必须可靠运行的可延期异步任务
androidx.work.Constraints.Builder
（可设定工作约束条件：比如联网、空闲、充电、存储空间充足）


### ----2020.4.8（庚子年三月十六）Wednesday -----

* 前端：
AsyncListUtil 是一个用于异步内容加载的类

> 60秒后过期倒计时器  
	android.os.CountDownTimer countDownTimer = new android.os.CountDownTimer(60000, 1000) 

android.os.CountDownTimer countDownTimer = new android.os.CountDownTimer(duration, delayTime) {
	@Override
	public void onTick(long millisUntilFinished) {
		
	}
	
	@Override
	public void onFinish() {
	
	}
};

ViewPager2+Fragment

类加载器
PathClassLoader
DexClassLoader

*在同一个类中，静态代码块与main函数中的代码谁先被执行？
>static类在程序装入内存时就要确定数据类型并分配内存，而main函数包括其中的变量是在执行到的时候才分配的。
静态代码块随着类的加载而执行，并且只执行一次，用于给类初始化，优先于主函数和方法。


java基础
Java 8 中我们可以通过 `::` 关键字来访问类的构造方法，对象方法，静态方法。



    import java.util.concurrent.atomic.AtomicLong;
    public class Main {
        static AtomicLong i = new AtomicLong();
    	//##静态块加载即执行，且只执行一次##
    	static {
    		//##加载类的时候，虚拟机会加锁保证只有一个线程去做加载动作
            //会一直等待
            //Thread t = new Thread(()->i.getAndIncrement());
            Thread t = new Thread(new Runnable() {
                @Override
                public void run() {
                    i.getAndIncrement();
                }
            });
            //可以顺利执行并打印1
            //Thread t = new Thread(i::getAndIncrement);
            t.start();
            try {
    			//此处挂起主线程执行子线程任务
                t.join();
            } catch (Exception e) {
                e.printStackTrace();
            }
        }		
    	//main一执行是开启一个进程，要加载各种资源，fork出很多线程，包括垃圾回收等线程
        public static void main(String[] a) {
            System.out.print(i.get());
        }
    }



lamada和死锁的问题，视频解释了：
[图片]https://www.bilibili.com/video/av59801808






后端：
RPC（Remote Procedure Call）远程过程调用

**ELK**

* Elasticsearch: 核心中的核心组件，基于著名的全文检索引擎lucence的一个分布式版本
* Logstash: 一个灵活的数据传输和处理系统，在beats出来之前，还负责进行数据收集。
* Kibana: 展示组件，基于angularjs。从Elasticsearch中读取数据并展示。

> 为何推出beats？

>Logstash在数据收集上并不出色，而且作为agent，性能并不达标。elastic发布了beats系列轻量级采集组件。




### ----2020.4.7（庚子年三月十五）Tuesday -------
jetpack-->paging分页库



git diff 版本编号1 版本编号2


JAVA 准备解析初始化！
https://mp.weixin.qq.com/s?__biz=MzIyNjUyNzQwMQ==&mid=2247483763&idx=1&sn=74fa1c054e91962b78f39c77b49425d6&scene=21#wechat_redirect


静态内部类的单例模式
https://mp.weixin.qq.com/s?src=3&timestamp=1586240207&ver=1&signature=DsLIvaPTLLx-RcdNB9eFfWz7UowM0CLpETMfT2WPLCLTkHsGCi4D9Te9N0*-jGFWnaAiDtiG-PhSLcbXM8dmQxbXtkT-KVGXXAe*vjw1RNJe-O7Uz8apcFLK1oMQ7JJ5L-QLgjpinMSlx7p-Pv3rgnzUgkvnMcmHkfSg5hyJ7jg=



** Facade与Mediator模式的区别？**
https://www.cnblogs.com/sweetdream/archive/2005/12/19/299983.html
Facade模式是解耦系统外到系统内（单向）的对象关联关系，
Mediator模式是解耦系统内各个对象之间在（双向）的关联关系


** 设计模式(17)--Mediator(中介者模式)行为型**
https://www.cnblogs.com/yysbolg/p/7518777.html
应用实例：
[1]Mediator模式在事件驱动类应用中比较多，例如聊天、消息传递等等，需要有一个MessageMediator，专门负责request/reponse之间任务的调节。
[2]MVC模式中，Controller是一种Mediator。
[3]JDK的具体应用：
　　　　　java.util.Timer
　　　　　java.util.concurrent.Executor#execute()
　　　　　java.util.concurrent.ExecutorService#submit()
　　　　　java.lang.reflect.Method#invoke()




优先级队列及小顶堆排序实现----【堆排序（大顶堆、小顶堆）】

LRU (最近最少使用) 缓存机制
LRU是Least Recently Used的缩写，即最近最少使用，是一种常用的页面置换算法，选择最近最久未使用的页面予以淘汰。


坦克大战设计模式有道云笔记链接
文档：tank_2019_v01
链接：http://note.youdao.com/noteshare?id=2231807fcb13c1d0fcbd4d63d63c3fe5

设计模式列表
https://note.youdao.com/ynoteshare1/index.html?id=2231807fcb13c1d0fcbd4d63d63c3fe5&type=notebook#/B7B2A3A1168644E08C5E69F3651F944E


思维导图绘制
https://www.processon.com/diagrams




### ----2020.4.6（庚子年三月十四）Monday -------
Room 持久性库
https://developer.android.google.cn/topic/libraries/architecture/room



微服务：拆分服务
单体应用架构-->微服务架构



### ----2020.4.5（庚子年三月十三）Sunday -------
Kafka
 MQ--->系统解耦、异步通信、削峰填谷
流式计算


TCP
    连接---三次握手
    断开---四次挥手




java.io
装饰器模式（Decorator）&&适配器模式（Adapter）
两个设计模式与IO框架的关联：
适配器模式主要在于字节流到字符流的转换和元素的包装上，
如类：InputStreamReader, CharArrayReader, FileReader, PipedReader, StringReader。

装饰模式主要在对流的强化之中，如缓冲、过滤、行定位等，
如类：BufferedReader, FilterReader, LineNumberReader。
FilterInputStream-DataInputStream,BufferedInputStream

举例说明：
BufferReader br = new BufferReader(new InputStreamReader(System.in));
上述把InputStream适配成InputStreamReader，再把InputStreamReader加强装饰城BufferedReader。



### ----2020.4.4（庚子年三月十二）Saturday -------
androidx.lifecycle包
Lifecycle
LiveData
MutableLiveData
ViewModel
https://developer.android.google.cn/topic/libraries/architecture/lifecycle#java



### ----2020.4.3（庚子年三月十一）Friday ------
报名享学课堂——> ￥5380
￥ 5380
￥10980
￥16360

AtomicReference

JVM垃圾回收：有向图机制 GC Roots
*引用计数法(弊端：很难解决对象之间的循环引用问题)
*枚举根节点做可达性分析


哪些对象可以作为 GC Roots 的对象？
*虚拟机栈中局部变量（也叫局部变量表）中引用的对象
*方法区中类的静态变量、常量引用的对象
*本地方法栈中 JNI (Native方法)引用的对象

解释：
gc1:是虚拟机栈中的局部变量
gc2:是方法区中类的静态变量
gc3:是方法区中的常量
都可以作为GC Roots 的对象。



Android内存泄露————非静态内部类|匿名内部类 默认持有外部类的引用


解决方案有2个思路：

一、严格保证程序逻辑。
		1.在销毁Activity的时候结束掉在执行的后台线程。线程结束了，就等于切断了与外部类关联的线。
		2.使用Handler.postDelayed( new Runnable(),xxx)方式的话，直接调用Handler的removeCallbacksAndMessages(null)方法，移除回收消息队列的消息即可。

二、采用静态内部类+弱引用（WeakReference）持有外部类实例

https://blog.csdn.net/u012982629/article/details/82770282




	at android.app.ActivityThread.main(ActivityThread.java:5151)
	at java.lang.reflect.Method.invokeNative(Method.java)
	at java.lang.reflect.Method.invoke(Method.java:515)
	at com.android.internal.os.ZygoteInit$MethodAndArgsCaller.run(ZygoteInit.java:868)
	at com.android.internal.os.ZygoteInit.main(ZygoteInit.java:684)
	at dalvik.system.NativeStart.main(NativeStart.java)


java.lang.String
intern()

为什么Java中synchronized同步的对象不能是Integer等类型？
原因是Java的自动封箱和解箱操作在作怪。
这里的i++实际上是i = new Integer(i+1)，所以执行完i++后，
i已经不是原来的对象了，同步块自然就无效了



java.util.concurrent.atomic
atomic是线程安全的基本数据类型
A small toolkit of classes that support lock-free thread-safe programming on single variables


Java纤程coroutine的实现(coroutine-libraries), 目前最好的应该还是Quasar

Quasar知识:Channel、Actor、Reactive Stream
Quasar官方参考文档
http://docs.paralleluniverse.co/quasar/



Zygote
Zygote 是Android第一个应用进程，它由init程序解析import /init.${ro.zygote}.rc 所启动。
在Android系统中，Zygote是java进程的鼻祖。它在启动时会创建虚拟机，并通过fork(复制进程)的形式来创建应用程序进程和SystemServer进程。

Zygote 由init.rc脚本解析启动。以下只考虑 Zygote 的启动而不考虑 init.rc 的解析。已知Zygote 的入口函数是app_main.cpp的main()函数。


***Glide源码分析****
***Glide生命周期管理
https://www.jianshu.com/p/317b2d6bde1b







### ----2020.4.2（庚子年三月初十）Thursday ------ 
Android图片轮播控件---com.youth.banner.Banner

优先级队列：根据时间先后顺序排队的单链表
handler.sendXXX
handler.sendXXX

Handler
	dispatchMessage(Message msg)
	enqueueMessage(MessageQueue queue, Message msg, long uptimeMillis)

	private boolean enqueueMessage(MessageQueue queue, Message msg, long uptimeMillis) {
		msg.target = this;//Handler
		if (mAsynchronous) {
			msg.setAsynchronous(true);
		}
		return queue.enqueueMessage(msg, uptimeMillis);
	}


一个线程是如何保证只有一个Looper？

	/**
	 * Get the map associated with a ThreadLocal. Overridden in
	 * InheritableThreadLocal.
	 *
	 * @param  t the current thread
	 * @return the map
	 */
	ThreadLocalMap getMap(Thread t) {
		return t.threadLocals;
	}



	// sThreadLocal.get() will return null unless you've called prepare().
	static final ThreadLocal<Looper> sThreadLocal = new ThreadLocal<Looper>()



	private static void prepare(boolean quitAllowed) {
		if (sThreadLocal.get() != null) {
			throw new RuntimeException("Only one Looper may be created per thread");
		}
		sThreadLocal.set(new Looper(quitAllowed));
	}

ThreadLocalMap维护ThreadLocal和Looper


Handler内存泄漏原因：
内存泄漏：生命周期不一致
非静态内部类持有外部类的引用


Handler持有上下文，message.target握住Handler



Handler--MessageQueue--Looper--


	/**
	 * Quits the looper safely.
	 * <p>
	 * Causes the {@link #loop} method to terminate as soon as all remaining messages
	 * in the message queue that are already due to be delivered have been handled.
	 * However pending delayed messages with due times in the future will not be
	 * delivered before the loop terminates.
	 * </p><p>
	 * Any attempt to post messages to the queue after the looper is asked to quit will fail.
	 * For example, the {@link Handler#sendMessage(Message)} method will return false.
	 * </p>
	 */
	public void quitSafely() {
		mQueue.quit(true);
	}

子线程中
prepare
loop
myHandler.looper.quitSafely();-->

释放内存、
释放子线程


synchronized:方法、静态方法、代码块(object)

代码块(this)

ThreadLocal源码解读
https://www.cnblogs.com/micrari/p/6790229.html

Java的synchronized的同步代码块和同步方法的区别
https://www.cnblogs.com/xujingyang/p/6565606.html



Message复用（享元模式）
/**

 * Recycles a Message that may be in-use.
 * Used internally by the MessageQueue and Looper when disposing of queued Messages.
 */
void recycleUnchecked() {

### ----2020.3.31（庚子年三月初八）Tuesday----

JetPack
ViewModel


[泛型:上界<? extends T>  vs 下界<? super T>](https://www.cnblogs.com/drizzlewithwind/p/6100164.html)  
PECS（Producer Extends Consumer Super）原则  
* 生产者：频繁往外读取内容的，适合用上界Extends（只读)
* 消费者：经常往里插入的，适合用下界Super

上界<? extends T>不能往里存，只能往外取
Plate<? extends Fruit> p=new Plate<Apple>(new Apple());

//不能存入任何元素
p.set(new Fruit());    //Error
p.set(new Apple());    //Error

//读取出来的东西只能存放在Fruit或它的基类里。
Fruit newFruit1=p.get();
Object newFruit2=p.get();
Apple newFruit3=p.get();    //Error

***
下界<? super T>不影响往里存，但往外取只能放在Object对象里  

	Plate<? super Fruit> p=new Plate<Fruit>(new Fruit());  
	//存入元素正常
	p.set(new Fruit());
	p.set(new Apple());
	//读取出来的东西只能存放在Object类里。
	Apple newFruit3=p.get();    //Error
	Fruit newFruit1=p.get();    //Error
	Object newFruit2=p.get();




----2020.3.30（庚子年三月初七）Monday----  
javapoet源代码生成



----2020.3.29（庚子年三月初六）Sunday----
梯子my.ishadowx.biz
Artifactory和
FIR/蒲公英

----2020.3.28（庚子年三月初五）Saturday----
动态代理
Java Proxy.newProxyInstance
CGLib是动态代理的经典类库

giflib动图处理

Java进阶Gradle系统详解
https://ke.qq.com/course/442126?taid=3857967258976014

### ----2020.3.27（庚子年三月初四）Friday----

androidx.core.app.ComponentActivity
androidx.appcompat.app.AppCompatActivity
com.android.internal.policy.PhoneWindow
androidx.core.view.KeyEventDispatcher

com.android.internal.policy.DecorView extends FrameLayout implements RootViewSurfaceTaker, WindowCallbacks

androidx.appcompat.view
android.view.Window.Callback
android.view.ViewRootImpl

android.os.Looper
android.os.Handler


java.lang.instrument包的最大功能就是可以在已有的类上附加（修改）字节码来实现增强的逻辑

javassist是一个开源的分析、编辑和创建java字节码的类库。通过使用javassist对字节码操作可以实现动态”AOP”框架。

java字节码处理工具：
bcel，asm(cglib只是对asm又封装了一层)，可以直接处理虚拟机指令
javassist的主要的优点，在于简单，而且快速，直接使用java编码的形式，而不需要了解虚拟机指令，就能动态改变类的结构，或者动态生成类。



### ----2020.3.25（庚子年三月初二）Monday----

JS异步编程之Promise



### ----2020.3.24（庚子年三月初一）Tuesday----

前端三大框架：
AngularJS(Google2009)、React(Facebook2013开源)、Vue.js(尤雨溪2014年2月)



### ----2020.3.23（庚子年二月三十）Monday----

okio：缓存机制
segment、segmentPool，对象池


Gson避免内存抖动
TypeAdapter+对象池

protobuf + mmkv
内存映射filechannel
***********

零拷贝技术分类
Linux 中的零拷贝技术主要有下面这几种：  
** 直接 I/O、mmap、sendfile、splice**

mars的日志模块 xlog


魔数：
魔数有两个含义
一指用来判断文件类型的魔数；
二指程序代码中的魔数，也称魔法值。


java代理（静态、动态）

java.lang.reflect
接口 InvocationHandler
public interface InvocationHandlerInvocationHandler 是代理实例的调用处理程序 实现的接口。
每个代理实例都具有一个关联的调用处理程序。对代理实例调用方法时，将对方法调用进行编码并将其指派到它的调用处理程序的 invoke 方法。
方法摘要
 Object invoke(Object proxy, Method method, Object[] args)
          在代理实例上处理方法调用并返回结果。

	************	  
java.lang.reflect
类 Proxy
java.lang.Object
  继承者 java.lang.reflect.Proxy

static Object newProxyInstance(ClassLoader loader, Class<?>[] interfaces, InvocationHandler h)  
创建某一接口 Foo 的代理（更简单的方法） ：
     Foo f = (Foo) Proxy.newProxyInstance(Foo.class.getClassLoader(),
                                          new Class[] { Foo.class },
                                          handler);

JAVA动态代理
参考资料：https://www.jianshu.com/p/9bcac608c714


java8中接口可以有实现方法 使用default修饰



面向对象的三大基本特征，五大基本原则
https://www.cnblogs.com/fzz9/p/8973315.html#%E4%BA%8C%E4%BA%94%E5%A4%A7%E5%9F%BA%E6%9C%AC%E5%8E%9F%E5%88%99

一、三大基本特征：封装、继承、多态
　　1、封装
　　2、继承
　　3、多态
四大特征的话，增加“抽象”特征
二、五大基本原则
　　1、单一职责原则（SRP）
　　2、开放封闭原则（OCP）
　　3、里氏替换原则（LSP）
　　4、依赖倒置原则（DIP）
　　5、接口隔离原则（ISP）



jsp八大内置对象
四大域，九大内置对象

### ----2020.3.22（庚子年二月廿九）Sunday----

java.lang.Class<T>
boolean isAssignableFrom(Class<?> cls)
 判定此 Class 对象所表示的类或接口与指定的 Class 参数所表示的类或接口是否相同，或是否是其超类或超接口



### ----2020.3.20（庚子年二月廿七）Fri-----
Proguard混淆注解@Keep



### ----2020.3.19（庚子年二月廿六）Thu-----

二进制表示法：大端、小端



MMKV—强大的存储工具
一款比sharepreferences稍重，远远小于数据库量级，但性能卓越的存储框架，由腾讯旗下的微信开发


SpUtil多样加密存储，兼容android9.0
http://www.demodashi.com/demo/15058.html

LiveEventBus
https://github.com/JeremyLiao/LiveEventBus/blob/master/docs/DIRECTION_1_3.md

### ----2020.3.17（庚子年二月廿四）Tue-----

CompletableFuture

Callable Future

FutureTask
java.util.concurrent.FutureTask<V>
类型参数：
V - 此 FutureTask 的 get 方法所返回的结果类型。
所有已实现的接口：
Runnable, Future<V>, RunnableFuture<V>
public class FutureTask<V> extends Object implements RunnableFuture<V>


public interface RunnableFuture<V>  extends Runnable, Future<V>
作为 Runnable 的 Future。成功执行 run 方法可以完成 Future 并允许访问其结果。



### ----2020.3.16（庚子年二月廿三）Mon-----

onTouch与onClick事件分发处理

DecorView处理事件  ViewGroup

### ----2020.3.15（庚子年二月廿二）Sunday----
Google Breakpad开源库来采集native的crash日志

jclasslib插件查看字节码



### ---2020.3.14（庚子年二月廿一）Saturday---

#Android组件化

apt 注解处理工具
javapoet源代码生成
AutoService注解

glide、eventbus、dagger

dex类加载、反射

dart语言开发库
https://pub.dev/

### ----2020.3.12（庚子年二月十九）Thu-----

 transient 关键字被用来表示变量将不被序列化处理

异步加载布局-AsyncLayoutInflater

### ----2020.3.11（庚子年二月十八）Wed-----

JAVA8 HashMap是由数组+链表+红黑树组成

将develop分支合并到master主干中
$git checkout master
$git merge develop


keyWord：张一鸣---延迟满足感

### ----2020.3.10（庚子年二月十七）Tue-----

public static Class<?> analysisClassInfo(Object object){
	//getGenericSuperclass可以得到包含原始类型，参数化类型，数组类型，类型变量，基本类型
	Type genType = object.getClass().getGenericSuperclass();
	//获取参数化类型(<Resule>)
	Type[] params = ((ParameterizedType) genType).getActualTypeArguments(); //强转换为参数类型
	return (Class<?>)params[0];
}

### --- 近4个月没有学习





>>遗憾啊，中途中断学习笔记近4个月 
>>
>>亡羊补牢，为时不晚
>>
>>亡羊补牢，为时不晚
>>
>>亡羊补牢，为时不晚
>>
>>亡羊补牢，为时不晚
>>
>>亡羊补牢，为时不晚
>>
>>亡羊补牢，为时不晚
>>
>>遗憾啊，中途中断学习笔记近4个月



### ---2019.11.9(己亥年十月十三) Saturday -----

未记录



### ---2019.11.3(己亥年十月初七) Sunday -----

未记录





### ---2019.11.2(己亥年十月初六) Saterday -----

**Android API --->HandlerThread**



***



### ---  近一周的没有学习记录

***





### ----2019.10.25（己亥年九月廿七）Fri-----



### ----2019.10.24（己亥年九月廿六）Thu-----

今日主要熟悉网易云信SDK


学习Python语法：
1、''、""、''' '''用法（打印皮卡丘）
2、str() int() float()方法
3、if elif else 语法（强制缩进）


重听bilibili网站Disruptor、RingBuffer讲座视频

### ----2019.10.23（己亥年九月廿五）Web-----

注解的原理：反射
retrofit：动态代理

Python学习
https://www.pypypy.cn/#/apps/1/lecture/5cd9765519bbcf0001554795


https://fir.im/docs/publish


发送消息到钉钉
https://ding-doc.dingtalk.com/doc#/serverapi2/qgx3dh

Google访问
https://crimson-boat-1577.minatoaqua.workers.dev/-----https://www.google.com/


Android开发：
api等同于废弃的compile等价于public
implementation   private
api和compile一样 可以在父项目引用

groovy语法
http://www.groovy-lang.org/style-guide.html#_omitting_parentheses
闭包

阿里maven仓库
https://maven.aliyun.com/mvn/view



本地仓库方案
nexus
代理方案
JFrog Artifactory Pro：支持maven、gradle
组件化

Repository	Key	Type	URL
aliyun_google m Maven https://maven.aliyun.com/repository/google
aliyun center https://maven.aliyun.com/repository/jcenter
aliyun public m Maven http: //maven.allyun.com/nexus/content/groups/public

让我们一起见证 Artifactory和 Retrofit在Gradle中的神奇效果吧
Domain specific language
移动架构师质
搬运工3,55,895%
中年危机加班
Grade 3.0 compile
Compile api public
implementation. Private
不负责任
基础
通用 Gradle android/ spring boot/ spring cloud
			artifactory ios/ android/php/java

1、完成这个插件; retrofit+gradle自动上传包到fir并且发送消息到丁丁
2、 github跑不起来;很慢; Artfactory pro

Gradle重要概念（从顶层到底层）
Plugin
Hooks
Tasks
Project
Closure
Wrapper

老师帮助我建立架构





Disruptor
https://blog.csdn.net/qq_19558705/article/details/77247912
	/ C1----\
P1<			  > C3
	\ C2----/
四边菱形任务、六边菱形任务执行



架构师技术图谱，助你早日成为架构师
https://github.com/toutiaoio/awesome-architecture?hmsr=toutiao.io&utm_medium=toutiao.io&utm_source=toutiao.io#282



### ----2019.10.22（己亥年九月廿四）Tue-----
Disruptor并发框架
https://www.bilibili.com/video/av57885285?from=search&seid=1251517418409342493

RingBuffer单独使用、
SequenceBarrier

坦克大战
Disruptor：

java基础知识和架构
模仿天猫整站SSM
http://how2j.cn?p=54321

### ----2019.10.21（己亥年九月廿三）Mon-----
数据结构可视化
https://visualgo.net/zh
https://www.geeksforgeeks.org/stack-data-structure/


访问量PV:(Page View)

TPS吞吐量(Throughput Per Second)：吞吐量是指系统在单位时间内处理请求的数量。

QPS每秒查询率(Query Per Second)
每秒查询率QPS是对一个特定的查询服务器在规定时间内所处理流量多少的衡量标准，在因特网上，作为域名系统服务器的机器的性能经常用每秒查询率来衡量。对应fetches/sec，即每秒的响应请求数，也即是最大吞吐能力。 （看来是类似于TPS，只是应用于特定场景的吞吐量）
QPS
原理：每天80%的访问集中在20%的时间里，这20%时间叫做峰值时间。
公式：( 总PV数 * 80% ) / ( 每天秒数 * 20% ) = 峰值时间每秒请求数(QPS) 。
机器：峰值时间每秒QPS / 单台机器的QPS = 需要的机器 。
每天300w PV 的在单台机器上，这台机器需要多少QPS？
( 3000000 * 0.8 ) / (86400 * 0.2 ) = 139 (QPS)。
一般需要达到139QPS，因为是峰值。



LMAX - How to Do 100K TPS at Less than 1ms Latency
https://www.infoq.com/presentations/LMAX/

https://lmax-exchange.github.io/disruptor/



吞吐量（TPS）、QPS、并发数、响应时间（RT）概念
https://www.cnblogs.com/longxiaojiangi/p/9259745.html

### ----2019.10.20（己亥年九月廿二）Sun-----
学车练习科目三路考
休息

###  ----2019.10.19（己亥年九月廿一）Sat-----
设计模式：
memento模式、
原型模式（Prototype）：实现cloneable接口clone的方法
JMH JAVA吞吐量测试开发利器
Disruptor简单入门


Guava的Optional
com.google.common.util.concurrent.RateLimiter.java

https://yq.aliyun.com/articles/665116?utm_content=m_1000022476

Android API
https://developer.android.google.cn/reference

JDK API
http://tool.oschina.net/apidocs/apidoc?api=jdk-zh

OPEN JDK
http://openjdk.java.net/

Google guava
https://github.com/google/guava

### ----2019.10.18（己亥年九月二十）Fri-----
RPC



treemap(红黑树)原理
TreeSet 底层实际使用的存储容器就是 TreeMap


ThreadPoolExecutor线程池
1、小于核心线程，直接新建线程
2、核心线程都在工作，加入任务队列
3、任务队列满了，新建非核心线程去执行
4、非核心线程满了且都在运行状态，若再有任务过来，则调用拒绝策略



设计模式：装饰者模式（Decorator pattern）
java.lang.Object
  继承者 java.io.InputStream
      继承者 java.io.FilterInputStream
所有已实现的接口：
Closeable
直接已知子类：
BufferedInputStream, CheckedInputStream, CipherInputStream, DataInputStream, DeflaterInputStream,
DigestInputStream, InflaterInputStream, LineNumberInputStream, ProgressMonitorInputStream, PushbackInputStream


范例：原型InputStream我们只能读取byte，现在直接从stream中读取int，String等类型
DataOutputStream dos = new DataOutputStream(new FileOutputStream("D:\\java.txt"));
dos.writeInt(1234567);
DataInputStream dis = new DataInputStream(new FileInputStream("D:\\java.txt"));
System.out.println(dis.readInt());
dis.close();
dos.close();

File file = new File("file.txt");
InputStream in =new BufferedInputStream(new FileInputStream(file), 512);
// 从字节流中读取5个字节。“abcde”，a对应0x61，b对应0x62，依次类推...
for (int i=0; i<len; if="">= 0) {
	// 读取“字节流的下一个字节”
	int tmp = in.read();
	System.out.printf("%d : 0x%s\n", i, Integer.toHexString(tmp));
	}
}


FileInputStream fileInputStream = new FileInputStream(new File("readme.txt"));
	BufferedInputStream bufferedInputStream = new BufferedInputStream(fileInputStream);
	byte[] bytes = new byte[1024];
	while(bufferedInputStream.read(bytes)!=-1){
		System.out.println(new String(bytes));
	}





### ----2019.10.17（己亥年九月十九）Thu-----
JUC学习
https://www.battleheart.cn

Online Judge
https://www.cnblogs.com/weiyinfu/p/10708677.html

CompletableFuture

Vector---HashTable 自带锁

DelayQueue：按照等待时间进行排序
PriorityQueue：优先队列

Queue对于线程友好的API,offer、peek、poll
BlockingQueue提供put、take阻塞方法（方便实现生产-消费者模型）

BlockingQueue：
LinkedBlockingQueue(无界队列）
ArrayBlockingQueue(有界队列)
队列满了
add阻塞
offer不阻塞直接返回false



底层阻塞是通过LockSupport.park()
ReentrantLock.


SynchronousQueue（同步队列）队列长度为0，专门用作线程间交换数据
TransferQueue（传递队列）装完--等待---取走

Exchanger.change

### ----2019.10.16（己亥年九月十八）Web-----
设计模式：Chain Of Responsibility
javax.servlet
Interface Filter
doFilter(ServletRequest request, ServletResponse response, FilterChain chain)
          The doFilter method of the Filter is called by the container each time a request/response pair is passed through the chain due to a client request for a resource at the end of the chain.

javax.servlet
Interface FilterChain



设计模式：
1、Iterator模式
2、Visitor模式----结合asm看visitor模式
3、Builder模式



ThreadLocal
WeakReference<M> m = new WeakReference<>(new M());
经过System.gc();后，m就被垃圾回收

作业：
WeakHashMap的用处
读AQS unlock的源码


ThreadLocal
	static class ThreadLocalMap
			static class Entry extends WeakReference<ThreadLocal<?>>
					Entry(ThreadLocal<?> k, Object v)



ThreadLocal<M> tl = new ThreadLocal<>();
tl.set(new M());
//!!!使用ThreadLocal之后，记得remove
tl.remove();



容器-Vector-Hashtable
CopyOnWriteList
ConcurrentHashMap
ConcurrentSkipListMap
BlockingQueue
目标：为ThreadPool做准备

### ----2019.10.15（己亥年九月十七）Tue-----
多线程高并发
redis
SpringCloud微服务

直播平台
客户端：obs studio
服务端：nginx+rtmp插件




设计模式：Adapter模式
 //将字节流转化为字符流
 InputStream in = new FileInputStream("C:/hello.txt");
 InputStreamReader isr = new InputStreamReader(in);

### ----2019.10.14（己亥年九月十六）Mon-----
知识点1：DevOps
 DevOps一词的来自于Development和Operations的组合，突出重视软件开发人员和运维人员的沟通合作，通过自动化流程来使得软件构建、测试、发布更加快捷、频繁和可靠。
 DevOps希望做到的是软件产品交付过程中IT工具链的打通，使得各个团队减少时间损耗，更加高效地协同工作。
 现代化的DevOps工具，如Chef、Docker、Ansible、Packer、Troposphere、Consul、Jenkins、SonarQube、AWS等

知识点：Netty
https://netty.io/wiki/related-articles.html
Netty:Bootstrap的handler和childHandler

netty官网概览
https://netty.io/4.0/xref/



学习目标：
有较扎实的Java基础知识，能够熟练使用Java相关技术进行独立开发；
熟悉Java多线程、并发库、熟悉TCP/IP协议，NIO，熟悉Netty框架，基础的算法和数据结构；
熟悉MySql数据库及MySql的优化，熟悉protobuf协议；
熟悉Maven构建工具；


精通Java，多线程编程，消息系统，数据库，分布式应用等技术，对SOA框架有较深刻的理解；
熟悉网络编程，具有设计和开发对外API接口经验和能力；
有Hadoop、Spark、Hive等相关经验者优先；



### ----2019.10.13（己亥年九月十五）Sun-----

netty客户端编程
BootStrap
EventLoopGroup接口实现类 NioEventLoopGroup（本质是一个线程池）

ChannelFuture
ChannelInitializer<SocketChannel>

Lombok插件

http://yapi.demo.qunar.com/
高效、易用、功能强大的API管理平台
旨在为开发、产品、测试人员提供更优雅的接口管理服务


1、Template模式
2、State模式？
3、Intepreter

### ----2019.10.12（己亥年九月十四）Sat-----
分布式系统
An Illustrated Proof of the CAP Theorem
https://mwhittaker.github.io/blog/an_illustrated_proof_of_the_cap_theorem/
Consistency 一致性
Availability 可用性
Partition tolerance 分区容错性

***
[java的动态代理机制详解](https://www.cnblogs.com/xiaoluo501395377/p/3383130.html)

InvocationHandler接口
	
	Object invoke(Object proxy, Method method, Object[] args) throws Throwable

proxy:　　指代我们所代理的那个真实对象
method:　　指代的是我们所要调用真实对象的某个方法的Method对象
args:　　指代的是调用真实对象某个方法时接受的参数

---------------------------------------------
proxy指的不是所代理的那个真实对象。如果是这样的话就没必要在handler中保存真实对象的引用了，，

在invoke中
System.out.println("proxy.getClass():" + proxy.getClass());
输出： proxy.getClass():class **com.sun.proxy.$Proxy0**

------------------------
* Proxy
	
	public static Object newProxyInstance(ClassLoader loader, Class<?>[] interfaces, InvocationHandler h) throws IllegalArgumentException
	

Proxy类加载器:

System.out.println("proxy.getClass().getClassLoader(): "+proxy.getClass().getClassLoader());
System.out.println("realSub.getClass().getClassLoader(): "+realSub.getClass().getClassLoader());

结果：
proxy.getClass().getClassLoader():		**sun.misc.Launcher$AppClassLoader@1471cb25**
realSub.getClass().getClassLoader():	**sun.misc.Launcher$AppClassLoader@1471cb25**

这两个的类加载器都是系统类加载器吧，应该一样的，所以用哪个都可以吧

另外，一共就只有**四种类加载器**，大家可以了解一下他们的加载机制
* 启动类加载器
* 扩展类加载器
* 系统类加载器
* 用户自定义类加载器
基本上我们能接触到的就只是**系统类加载器**

***


Proxy模式：
JDK动态代理    关键API:Proxy InvocationHandler  缺点：被代理对象必须实现接口
cglib动态代理  关键API:Enhancer+MethodInterceptor 优点：被代理对象无需实现接口，使用简单 缺点：不能代理final对象
org.objectweb.asm 小而快速的字节码操作框架     缺点：直接修改字节码，使用复杂
asm官网
https://gitlab.ow2.org/asm/asm
https://asm.ow2.io/





javaassist简要介绍
和AOP有什么关系和区别？CGLib是动态代理的经典类库，其底层实现使用ASM

Java bytecode engineering toolkit http://www.javassist.org
javassist底层实现类似ASM
Javassist (JAVA programming ASSISTant) 是在 Java 中编辑字节码的类库;它使 Java 程序能够在运行时定义一个新类, 并在 JVM 加载时修改类文件。
我们常用到的动态特性主要是反射，在运行时查找对象属性、方法，修改作用域，通过方法名称调用方法等。
在线的应用不会频繁使用反射，因为反射的性能开销较大。其实还有一种和反射一样强大的特性，但是开销却很低，它就是Javassit。
与其他类似的字节码编辑器不同, Javassist 提供了两个级别的 API: 源级别和字节码级别。
如果用户使用源级 API, 他们可以编辑类文件, 而不知道 Java 字节码的规格。 整个 API 只用 Java 语言的词汇来设计。 您甚至可以以源文本的形式指定插入的字节码; Javassist 在运行中编译它


java.lang.instrument

提供允许 Java 编程语言代理检测运行在 JVM 上的程序的服务



多线程高并发
java.util.concurrent
Interface Future<V>

java.util.concurrent
Interface Callable<V>


java.util.concurrent
Class FutureTask<V>
All Implemented Interfaces:Runnable, Future<V>, RunnableFuture<V>

### ----2019.10.11（己亥年九月十三）Fri-----

GoF《设计模式》
Facade模式（封装内部逻辑细节，对外提供简化接口）
Decorator模式：不改变原对象的前提下，扩展原对象的功能（不使用继承）
	File f1 = new File("D:\\Rain.txt");
	FileInputStream fis = new FileInputStream(f1);
	BufferedInputStream bis = new BufferedInputStream(fis);//为FileInputStream增加了缓冲功能



Proxy模式：

WeakHashMap



栈stack内存--->存储函数的主体和变量名
堆heap内存---->堆内存是用来存储实例(实例化后的对象实体)的
引用名都放在栈内存,值放堆内存

栈内存是线程私有的，堆内存是公共的



### ----2019.10.10（己亥年九月十二）Thu-----
报名马士兵教育-->￥10980元
VarHandle
java四种引用：强、软、弱、虚
    软引用和弱引用的价值：
    适合保存那些可有可无的缓存数据，当内存不足时，缓存数据被回收（再通过备选方案查询），当内存充足时，也可以存在较长时间，起到加速的作用。
异或位操作
容器