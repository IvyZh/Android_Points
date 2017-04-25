# RxJava 入门

## 1.观察者模式理论篇

- 什么是观察者模式？

![](http://1)

- 观察者模式UML

![](http://2)

- 总结

![](http://3)

## 2.观察者模式动手篇

- Observer-->接口(interface)

![](http://5)

- Subject-->抽象类(abstract)
	- 存放观察者集合ArrayList<Observer>
	- attach(Observer observer):添加观察者
	- dettch(Observer observer)：删除观察者
	- notifyObserver(String state):通知所有观察者状态已经发生改变,遍历Observer集合，调用update(state)方法

![](http://4)

- 创建Observer子类SunnyObserver

![](http://6)

- 创建Subject的子类MassageSubject

![](http://7)


- 调用

![](http://8)


Android中的应用就是点击事件的监听

attach 相当于setListener

- Java中也有类是的Observer和Observable

![](http://9)


## 3.课程大纲介绍


> 学习路线 Okhttp3--->Retrofit2--->RxJava2--->Dragger2--->EventBus--->DataBanding


- 如何学习？
	- 官方文档
	- 
## 4.基本使用
## 5.线程控制
## 6.操作符介绍
## 7.登录后获取用户信息
## 8.关键词搜索案例
## 9.防止按钮重复点击案例
## 10.购物车合并本地和网络数据的案例
## 11.发送验证码倒计时案例
## 12.自定义图片缓存框架-1
## 13.自定义图片缓存框架-2
## 14.自定义图片缓存框架-3
--------------



