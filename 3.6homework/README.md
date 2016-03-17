#3.6HomeWork by fanl

##1、反编译任意apk，并且截图；
将apk修改为.zip
解压缩后拷贝classes.dex文件至dex2jar目录下
使用cmd cd到该目录下
输入d2j-dex2jar.bat    classes.dex后，查看目录下，生成了classes-dex2jar.jar
使用jd-gui打开查看源码
![](http://i.imgur.com/5Lzp3Ln.png)
![](http://i.imgur.com/37EmIKV.png)
##2、使用aapt的命令查询权限，并且截图；
aapt dump permissions xx.apk
![](http://i.imgur.com/moPSXVx.png)
##3、编写3种不同切入点的Android monkey的命令，并成功运行，同时说明切入点是什么；

##4、请找出Android monkey中motion和touch对应的源码里的方法，并找出monkey工具实现点击的最基础发方法是什么；
![](http://i.imgur.com/JgJoxuv.png)
![](http://i.imgur.com/nS39qRY.png)
点击最基础方法：

##5、找到任意一个apk or ipa，然后去寻找里面的db，并打开，上传截图；
使用root后的Android手机，使用adb pull 命令将data/data/packagename目录下的文件保存至PC本地，找到db文件，使用db查看工具sqlite developer打开db并查看db中的表是否被加密
![](http://i.imgur.com/r6kXixQ.png)

##6、（mac专享）github上去找monkey.js 去instruments运行，给出instruments运行的结果图；

##7、（mac专享）安装idevicestaller，获取iOS日志；