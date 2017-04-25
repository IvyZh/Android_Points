# RxJava 入门

> 2016.11

## 1.观察者模式理论篇

- 什么是观察者模式？

![](https://github.com/IvyZh/Android_Points/blob/master/imgs/rxjava2/QQ%E6%88%AA%E5%9B%BE20170425103655.jpg)


- 观察者模式UML

![](https://github.com/IvyZh/Android_Points/blob/master/imgs/rxjava2/QQ%E6%88%AA%E5%9B%BE20170425103713.jpg)


- 总结
![](https://github.com/IvyZh/Android_Points/blob/master/imgs/rxjava2/QQ%E6%88%AA%E5%9B%BE20170425103801.jpg)


## 2.观察者模式动手篇

- Observer-->接口(interface)

![](https://github.com/IvyZh/Android_Points/blob/master/imgs/rxjava2/QQ%E6%88%AA%E5%9B%BE20170425104629.jpg)


- Subject-->抽象类(abstract)
	- 存放观察者集合ArrayList<Observer>
	- attach(Observer observer):添加观察者
	- dettch(Observer observer)：删除观察者
	- notifyObserver(String state):通知所有观察者状态已经发生改变,遍历Observer集合，调用update(state)方法


![](https://github.com/IvyZh/Android_Points/blob/master/imgs/rxjava2/QQ%E6%88%AA%E5%9B%BE20170425104538.jpg)

- 创建Observer子类SunnyObserver

![](https://github.com/IvyZh/Android_Points/blob/master/imgs/rxjava2/QQ%E6%88%AA%E5%9B%BE20170425104855.jpg)


- 创建Subject的子类MassageSubject

![](https://github.com/IvyZh/Android_Points/blob/master/imgs/rxjava2/QQ%E6%88%AA%E5%9B%BE20170425104957.jpg)



- 调用

![](https://github.com/IvyZh/Android_Points/blob/master/imgs/rxjava2/QQ%E6%88%AA%E5%9B%BE20170425105228.jpg)



Android中的应用就是点击事件的监听

attach 相当于setListener

- Java中也有类是的Observer和Observable

![](https://github.com/IvyZh/Android_Points/blob/master/imgs/rxjava2/QQ%E6%88%AA%E5%9B%BE20170425105602.jpg)

## 3.课程大纲介绍


> 学习路线 Okhttp3--->Retrofit2--->RxJava2--->Dragger2--->EventBus--->DataBanding


- 如何学习？
	- 官方文档
	- Google
	- 结合实际项目


- RxJava课程大纲
	- 观察者模式讲解
	- 基本使用
	- 线程控制
	- 操作符（案例）！！
		- 防止重复点击
		- 注册时输入项（邮箱、密码、电话等）合法时点亮注册按钮
		- 合并两组数据一起展示（网络和本地）、购物车
		- 关键词搜索 避免频繁请求网络
		- 数据缓存 检查Memory、disk和network
		- 倒计时-发送短信按钮倒计时结束后恢复可用
		- 每隔5秒中检查新消息


## 4.基本使用

![](http://10)
![](http://11)

步骤

![](http://12)

![](http://13)

![](http://14)

更简洁的写法：
![](http://15)

代码：

![](http://16)

![](http://17)

其他用法：

- 被观察者：

![](http://18)

![](http://19)


## 5.线程控制

![](http://20)
![](http://21)
![](http://22)

## 6.操作符介绍

- Operator
	- 创建操作符
		- Create
		- Just
		- From	
	- 变换操作符（数据类型的转换）
		- FlatMap
		- Map
	- 过滤操作
		- Distinct
		- Filter
	- 结合操作
		- Join
	- 错误
	- 辅助
	- 条件和布尔
	- 算术和聚合
	- 异步
	- 连接
	- ...


## 7.登录后获取用户信息


> Map  操作符对原始Observable发射的每一项数据应用一个你选择的函数，然后返回一个发射
这些结果的Observable

![](http://23)


案例：登录后获取用户信息

用到FlatMap：

> FlatMap  将一个发射数据的Observable变换为多个Observables，然后将它们发射的数据合并
后放进一个单独的Observable

先用最原始的方式：

![](http://24)

![](http://25)

![](http://26)

线程切换：

![](http://27)


注意：

![](http://28)

![](http://29)

需要加上适配

这样的话，只需要这么设置了
![](http://30)

## 8.关键词搜索案例

![](http://31)
操作符：Debounce

> 仅在过了一段指定时间还没发射数据时才发射一个数据

> RxBinding

rxbinding 0.4.0 使用的是rxjava1.0 所以要去掉2.0的gradle

![](http://32)

![](http://33)

过滤数据：比如搜索条件为空的时候就不需要发起网络请求了

![](http://34)

如何防止数据被覆盖？

switchMap和flatMap使用方法是一样的，只不过switchMap只保留最后一次发射的数据

## 9.防止按钮重复点击案例

![](http://35)

![](http://36)

## 10.购物车合并本地和网络数据的案例

![](http://37)

![](http://38)

![](http://39)

## 11.发送验证码倒计时案例

CountDownTime 也可以实现

使用RxJava操作符interval

![](http://40)

时间问题

![](http://41)

## 12.自定义图片缓存框架-1

![](http://42)

processon.com

使用RxJava来实现三级缓存

数据源看做是Observable，使用最近的

![](http://43)

![](http://44)

## 13.自定义图片缓存框架-2

使用效果：

![](http://45)



## 14.自定义图片缓存框架-3
--------------



