## ssh翻墙

有时候yum下载太慢了，需要个梯子。

### 1.首先得到一个ssr

### 2.ssr开启允许局域网连接

首先右键点击小飞机，点击【选项设置】

![image-20201216171420457](E:%5C%E5%B7%A5%E4%BD%9C%5C%E6%A1%A3%E6%A1%88%5Cmd%E5%9B%BE%E5%BA%8A%5Cimage-20201216171420457.png) 

然后勾选允许局域网连接就可以，端口可以自定义一个不冲突的端口

![image-20201216171437641](E:%5C%E5%B7%A5%E4%BD%9C%5C%E6%A1%A3%E6%A1%88%5Cmd%E5%9B%BE%E5%BA%8A%5Cimage-20201216171437641.png) 



### 3.shell工具翻墙

```shell
export ALL_PROXY=sock5://xx.xx.xx.xx:yy
#其中xx.xx.xx.xx是开了ssr的服务器地址
#yy是指定的端口
```



执行后可以和google通信

![image-20201216171454411](E:%5C%E5%B7%A5%E4%BD%9C%5C%E6%A1%A3%E6%A1%88%5Cmd%E5%9B%BE%E5%BA%8A%5Cimage-20201216171454411.png) 