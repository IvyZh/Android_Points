# OkHttp3 入门

> 2016.10

## 1.快速使用
github website

![](https://github.com/IvyZh/Android_Points/blob/master/imgs/okhttp3/QQ%E6%88%AA%E5%9B%BE20170425113830.jpg)

Get请求快速入门

![](https://github.com/IvyZh/Android_Points/blob/master/imgs/okhttp3/QQ%E6%88%AA%E5%9B%BE20170425114449.jpg)

## 2.Http协议介绍

- Http是什么？

![](https://github.com/IvyZh/Android_Points/blob/master/imgs/okhttp3/QQ%E6%88%AA%E5%9B%BE20170425131534.jpg)
![](https://github.com/IvyZh/Android_Points/blob/master/imgs/okhttp3/QQ%E6%88%AA%E5%9B%BE20170425131547.jpg)
![](https://github.com/IvyZh/Android_Points/blob/master/imgs/okhttp3/QQ%E6%88%AA%E5%9B%BE20170425131608.jpg)

- 什么是URL？

![](https://github.com/IvyZh/Android_Points/blob/master/imgs/okhttp3/QQ%E6%88%AA%E5%9B%BE20170425131618.jpg)
![](https://github.com/IvyZh/Android_Points/blob/master/imgs/okhttp3/QQ%E6%88%AA%E5%9B%BE20170425131723.jpg)

- Request

![](https://github.com/IvyZh/Android_Points/blob/master/imgs/okhttp3/QQ%E6%88%AA%E5%9B%BE20170425131745.jpg)
![](https://github.com/IvyZh/Android_Points/blob/master/imgs/okhttp3/QQ%E6%88%AA%E5%9B%BE20170425131820.jpg)


- Response

![](https://github.com/IvyZh/Android_Points/blob/master/imgs/okhttp3/QQ%E6%88%AA%E5%9B%BE20170425131840.jpg)

- Http协议请求方法

![](https://github.com/IvyZh/Android_Points/blob/master/imgs/okhttp3/QQ%E6%88%AA%E5%9B%BE20170425131931.jpg)




- Get和Post方法的区别

![](https://github.com/IvyZh/Android_Points/blob/master/imgs/okhttp3/QQ%E6%88%AA%E5%9B%BE20170425131949.jpg)


- 状态码
![](https://github.com/IvyZh/Android_Points/blob/master/imgs/okhttp3/QQ%E6%88%AA%E5%9B%BE20170425132022.jpg)
![](https://github.com/IvyZh/Android_Points/blob/master/imgs/okhttp3/QQ%E6%88%AA%E5%9B%BE20170425132044.jpg)
![](https://github.com/IvyZh/Android_Points/blob/master/imgs/okhttp3/QQ%E6%88%AA%E5%9B%BE20170425132059.jpg)


## 3.Get请求（获取用户信息为例）

![](https://github.com/IvyZh/Android_Points/blob/master/imgs/okhttp3/QQ%E6%88%AA%E5%9B%BE20170425133128.jpg)

![](https://github.com/IvyZh/Android_Points/blob/master/imgs/okhttp3/QQ%E6%88%AA%E5%9B%BE20170425133213.jpg)

## 4.Post请求（Form表单形式）

![](https://github.com/IvyZh/Android_Points/blob/master/imgs/okhttp3/QQ%E6%88%AA%E5%9B%BE20170425133447.jpg)
![](https://github.com/IvyZh/Android_Points/blob/master/imgs/okhttp3/QQ%E6%88%AA%E5%9B%BE20170425133703.jpg)
![](https://github.com/IvyZh/Android_Points/blob/master/imgs/okhttp3/QQ%E6%88%AA%E5%9B%BE20170425133805.jpg)




## 5.Post请求（JSON参数形式）

![](https://github.com/IvyZh/Android_Points/blob/master/imgs/okhttp3/QQ%E6%88%AA%E5%9B%BE20170425134136.jpg)


## 6.文件下载（简单方式）

- 文件下载两种方式
	- 流读取
	- 拦截器

- 流读取方式


![](https://github.com/IvyZh/Android_Points/blob/master/imgs/okhttp3/QQ%E6%88%AA%E5%9B%BE20170425134601.jpg)
![](https://github.com/IvyZh/Android_Points/blob/master/imgs/okhttp3/QQ%E6%88%AA%E5%9B%BE20170425134831.jpg)
![](https://github.com/IvyZh/Android_Points/blob/master/imgs/okhttp3/QQ%E6%88%AA%E5%9B%BE20170425134850.jpg)

![](https://github.com/IvyZh/Android_Points/blob/master/imgs/okhttp3/QQ%E6%88%AA%E5%9B%BE20170425135030.jpg)
![](https://github.com/IvyZh/Android_Points/blob/master/imgs/okhttp3/QQ%E6%88%AA%E5%9B%BE20170425135130.jpg)


## 7.文件下载（拦截器方式）

- 拦截器方式

简书-对于wiki 拦截器的翻译文章《OkHttp-wiki之Interceptors拦截器》


自定义ResponseBody继承ResponseBody


- ProgressResponseBody

![](https://github.com/IvyZh/Android_Points/blob/master/imgs/okhttp3/QQ%E6%88%AA%E5%9B%BE20170425141003.jpg)
![](https://github.com/IvyZh/Android_Points/blob/master/imgs/okhttp3/QQ%E6%88%AA%E5%9B%BE20170425141051.jpg)
![](https://github.com/IvyZh/Android_Points/blob/master/imgs/okhttp3/QQ%E6%88%AA%E5%9B%BE20170425141101.jpg)


- 进度监听Listener

![](https://github.com/IvyZh/Android_Points/blob/master/imgs/okhttp3/QQ%E6%88%AA%E5%9B%BE20170425141227.jpg)


- 拦截器使用

![](https://github.com/IvyZh/Android_Points/blob/master/imgs/okhttp3/QQ%E6%88%AA%E5%9B%BE20170425141408.jpg)


- 读写文件

![](https://github.com/IvyZh/Android_Points/blob/master/imgs/okhttp3/QQ%E6%88%AA%E5%9B%BE20170425141550.jpg)
![](https://github.com/IvyZh/Android_Points/blob/master/imgs/okhttp3/QQ%E6%88%AA%E5%9B%BE20170425141630.jpg)

注：也可以使用拦截器实现文件写到本地

## 8.OkHttp简单封装1
## 9.OkHttp简单封装2

> 有时间再好好看看这两节的封装思想。

--------------
end.



