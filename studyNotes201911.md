##----------2020.4.11（庚子年三月十九）Saturday---------
CLion
CLion: A Cross-Platform IDE for C and C++ by JetBrains



##----------2020.4.10（庚子年三月十八）Friday---------

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


##----------2020.4.9（庚子年三月十七）Thursday---------

**自定义View**
	ViewRootImpl.performTransversal

##前端-JetPack系列
androidx.work.WorkManager
调度必须可靠运行的可延期异步任务
androidx.work.Constraints.Builder
（可设定工作约束条件：比如联网、空闲、充电、存储空间充足）


##----------------2020.4.8（庚子年三月十六）Wednesday----------------------------------------

* 前端：
AsyncListUtil 是一个用于异步内容加载的类

>60秒后过期倒计时器
  android.os.CountDownTimer countDownTimer = new CountDownTimer(60000, 1000) 

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




##----------------2020.4.7（庚子年三月十五）Tuesday---------------------------------------------
jetpack-->paging分页库



git diff 版本编号1 版本编号2


JAVA 准备解析初始化！
https://mp.weixin.qq.com/s?__biz=MzIyNjUyNzQwMQ==&mid=2247483763&idx=1&sn=74fa1c054e91962b78f39c77b49425d6&scene=21#wechat_redirect


静态内部类的单例模式
https://mp.weixin.qq.com/s?src=3&timestamp=1586240207&ver=1&signature=DsLIvaPTLLx-RcdNB9eFfWz7UowM0CLpETMfT2WPLCLTkHsGCi4D9Te9N0*-jGFWnaAiDtiG-PhSLcbXM8dmQxbXtkT-KVGXXAe*vjw1RNJe-O7Uz8apcFLK1oMQ7JJ5L-QLgjpinMSlx7p-Pv3rgnzUgkvnMcmHkfSg5hyJ7jg=



#### Facade与Mediator模式的区别？
https://www.cnblogs.com/sweetdream/archive/2005/12/19/299983.html
Facade模式是解耦系统外到系统内（单向）的对象关联关系，
Mediator模式是解耦系统内各个对象之间在（双向）的关联关系


### 设计模式(17)--Mediator(中介者模式)行为型
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




##----------------2020.4.6（庚子年三月十四）Monday---------------------------------------------
Room 持久性库
https://developer.android.google.cn/topic/libraries/architecture/room



微服务：拆分服务
单体应用架构-->微服务架构



##----------------2020.4.5（庚子年三月十三）Sunday---------------------------------------------
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



##----------------2020.4.4（庚子年三月十二）Saturday---------------------------------------------
androidx.lifecycle包
Lifecycle
LiveData
MutableLiveData
ViewModel
https://developer.android.google.cn/topic/libraries/architecture/lifecycle#java



##----------------2020.4.3（庚子年三月十一）Friday---------------------------------------------
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










-----------2020.4.2（庚子年三月初十）Thursday-----------------
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

----2020.3.31（庚子年三月初八）Tuesday----
JetPack
ViewModel



PECS（Producer Extends Consumer Super）原则
频繁往外读取内容的，适合用上界Extends。
经常往里插入的，适合用下界Super

上界<? extends T>不能往里存，只能往外取
Plate<? extends Fruit> p=new Plate<Apple>(new Apple());

//不能存入任何元素
p.set(new Fruit());    //Error
p.set(new Apple());    //Error

//读取出来的东西只能存放在Fruit或它的基类里。
Fruit newFruit1=p.get();
Object newFruit2=p.get();
Apple newFruit3=p.get();    //Error

*******分割*******
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


----2020.3.27（庚子年三月初四）Friday----
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



----2020.3.25（庚子年三月初二）Monday----
JS异步编程之Promise



----2020.3.24（庚子年三月初一）Tuesday----
前端三大框架：
AngularJS(Google2009)、React(Facebook2013开源)、Vue.js(尤雨溪2014年2月)



----2020.3.23（庚子年二月三十）Monday----

okio：缓存机制
segment、segmentPool，对象池


Gson避免内存抖动
TypeAdapter+对象池

protobuf + mmkv
内存映射filechannel
***********

零拷贝技术分类
Linux 中的零拷贝技术主要有下面这几种：
直接 I/O、mmap、sendfile、splice
-------
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


----2020.3.22（庚子年二月廿九）Sunday----
java.lang.Class<T>
boolean isAssignableFrom(Class<?> cls)
 判定此 Class 对象所表示的类或接口与指定的 Class 参数所表示的类或接口是否相同，或是否是其超类或超接口



-------2020.3.20（庚子年二月廿七）Fri---------
Proguard混淆注解@Keep


-------2020.3.19（庚子年二月廿六）Thu---------
二进制表示法：大端、小端



MMKV—强大的存储工具
一款比sharepreferences稍重，远远小于数据库量级，但性能卓越的存储框架，由腾讯旗下的微信开发


SpUtil多样加密存储，兼容android9.0
http://www.demodashi.com/demo/15058.html

LiveEventBus
https://github.com/JeremyLiao/LiveEventBus/blob/master/docs/DIRECTION_1_3.md

-------2020.3.17（庚子年二月廿四）Tue---------
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



-------2020.3.16（庚子年二月廿三）Mon---------
onTouch与onClick事件分发处理

DecorView处理事件  ViewGroup

----2020.3.15（庚子年二月廿二）Sunday----
Google Breakpad开源库来采集native的crash日志

jclasslib插件查看字节码



---2020.3.14（庚子年二月廿一）Saturday---

#Android组件化

apt 注解处理工具
javapoet源代码生成
AutoService注解

glide、eventbus、dagger

dex类加载、反射

dart语言开发库
https://pub.dev/


-------2020.3.12（庚子年二月十九）Thu---------
 transient 关键字被用来表示变量将不被序列化处理

异步加载布局-AsyncLayoutInflater


-------2020.3.11（庚子年二月十八）Wed---------
JAVA8 HashMap是由数组+链表+红黑树组成

将develop分支合并到master主干中
$git checkout master
$git merge develop


keyWord：张一鸣---延迟满足感

-------2020.3.10（庚子年二月十七）Tue---------
public static Class<?> analysisClassInfo(Object object){
	//getGenericSuperclass可以得到包含原始类型，参数化类型，数组类型，类型变量，基本类型
	Type genType = object.getClass().getGenericSuperclass();
	//获取参数化类型(<Resule>)
	Type[] params = ((ParameterizedType) genType).getActualTypeArguments(); //强转换为参数类型
	return (Class<?>)params[0];
}



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



`----------2019年11月9日 Saturday---------`



`----------2019年11月3日 Sunday---------`


`----------2019年11月2日 Saterday---------`

**Android API --->HandlerThread**




-------2019.10.24（己亥年九月廿七）Fri---------




-------2019.10.24（己亥年九月廿六）Thu---------

今日主要熟悉网易云信SDK


学习Python语法：
1、''、""、''' '''用法（打印皮卡丘）
2、str() int() float()方法
3、if elif else 语法（强制缩进）


重听bilibili网站Disruptor、RingBuffer讲座视频

-------2019.10.23（己亥年九月廿五）Web---------

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



-------2019.10.22（己亥年九月廿四）Tue---------
Disruptor并发框架
https://www.bilibili.com/video/av57885285?from=search&seid=1251517418409342493

RingBuffer单独使用、
SequenceBarrier

坦克大战
Disruptor：

java基础知识和架构
模仿天猫整站SSM
http://how2j.cn?p=54321


-------2019.10.21（己亥年九月廿三）Mon---------
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

-------2019.10.20（己亥年九月廿二）Sun---------
学车练习科目三路考
休息

-------2019.10.19（己亥年九月廿一）Sat---------
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

-------2019.10.18（己亥年九月二十）Fri---------
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






-------2019.10.17（己亥年九月十九）Thu---------
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


-------2019.10.16（己亥年九月十八）Web---------
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


-------2019.10.15（己亥年九月十七）Tue---------
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

-------2019.10.14（己亥年九月十六）Mon---------
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




-------2019.10.13（己亥年九月十五）Sun---------
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


-------2019.10.12（己亥年九月十四）Sat---------
分布式系统
An Illustrated Proof of the CAP Theorem
https://mwhittaker.github.io/blog/an_illustrated_proof_of_the_cap_theorem/
Consistency 一致性
Availability 可用性
Partition tolerance 分区容错性







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

-------2019.10.11（己亥年九月十三）Fri---------
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



-------2019.10.10（己亥年九月十二）Thu---------
VarHandle
java四种引用：强、软、弱、虚
    软引用和弱引用的价值：
    适合保存那些可有可无的缓存数据，当内存不足时，缓存数据被回收（再通过备选方案查询），当内存充足时，也可以存在较长时间，起到加速的作用。
异或位操作
容器
