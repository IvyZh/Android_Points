# RxJava 入门

> 2016.10

## 1.基本介绍
website


## 2.快速上手体验

- Call<ResponseBody>

配置API

![](https://github.com/IvyZh/Android_Points/blob/master/imgs/retrofit2/QQ%E6%88%AA%E5%9B%BE20170425154936.jpg)


使用

![](https://github.com/IvyZh/Android_Points/blob/master/imgs/retrofit2/QQ%E6%88%AA%E5%9B%BE20170425155033.jpg)



- Call<User>

![](https://github.com/IvyZh/Android_Points/blob/master/imgs/retrofit2/QQ%E6%88%AA%E5%9B%BE20170425155119.jpg)
![](https://github.com/IvyZh/Android_Points/blob/master/imgs/retrofit2/QQ%E6%88%AA%E5%9B%BE20170425155148.jpg)


报错：转换器

![](https://github.com/IvyZh/Android_Points/blob/master/imgs/retrofit2/QQ%E6%88%AA%E5%9B%BE20170425155207.jpg)


配置Gson转换器

![](https://github.com/IvyZh/Android_Points/blob/master/imgs/retrofit2/QQ%E6%88%AA%E5%9B%BE20170425155241.jpg)


## 3.GET请求介绍

@Query

@Path

@QueryMap


## 4.Post请求介绍

- Json
	- @Body
- Form
	- @FormUrlEncoded
	- @Field
	- @Multipart
	- @Part



- Json形式

![](https://github.com/IvyZh/Android_Points/blob/master/imgs/retrofit2/QQ%E6%88%AA%E5%9B%BE20170425160159.jpg)
![](https://github.com/IvyZh/Android_Points/blob/master/imgs/retrofit2/QQ%E6%88%AA%E5%9B%BE20170425160315.jpg)


- Form表单形式

![](https://github.com/IvyZh/Android_Points/blob/master/imgs/retrofit2/QQ%E6%88%AA%E5%9B%BE20170425160500.jpg)
![](https://github.com/IvyZh/Android_Points/blob/master/imgs/retrofit2/QQ%E6%88%AA%E5%9B%BE20170425160522.jpg)
![](https://github.com/IvyZh/Android_Points/blob/master/imgs/retrofit2/QQ%E6%88%AA%E5%9B%BE20170425160634.jpg)


修改头信息

![](https://github.com/IvyZh/Android_Points/blob/master/imgs/retrofit2/QQ%E6%88%AA%E5%9B%BE20170425160858.jpg)
![](https://github.com/IvyZh/Android_Points/blob/master/imgs/retrofit2/QQ%E6%88%AA%E5%9B%BE20170425160927.jpg)



## 5.与RxJava结合使用

步骤

![](https://github.com/IvyZh/Android_Points/blob/master/imgs/retrofit2/QQ%E6%88%AA%E5%9B%BE20170425161135.jpg)

![](https://github.com/IvyZh/Android_Points/blob/master/imgs/retrofit2/QQ%E6%88%AA%E5%9B%BE20170425161220.jpg)


需求：调用登陆接口，登陆成功之后根据返回的用户id，在调用获取用户信息的接口


普通方式：

![](https://github.com/IvyZh/Android_Points/blob/master/imgs/retrofit2/QQ%E6%88%AA%E5%9B%BE20170425161433.jpg)
![](https://github.com/IvyZh/Android_Points/blob/master/imgs/retrofit2/QQ%E6%88%AA%E5%9B%BE20170425161521.jpg)


使用RxJava方式：

![](https://github.com/IvyZh/Android_Points/blob/master/imgs/retrofit2/QQ%E6%88%AA%E5%9B%BE20170425161903.jpg)
![](https://github.com/IvyZh/Android_Points/blob/master/imgs/retrofit2/QQ%E6%88%AA%E5%9B%BE20170425161951.jpg)


还有一种方式：

![](https://github.com/IvyZh/Android_Points/blob/master/imgs/retrofit2/QQ%E6%88%AA%E5%9B%BE20170425162216.jpg)



运行报错：不能在主线程进行网络操作

线程控制：

![](https://github.com/IvyZh/Android_Points/blob/master/imgs/retrofit2/QQ%E6%88%AA%E5%9B%BE20170425162455.jpg)


--------------



