# git
+ 克隆項目到本地： git clone url path


# linux
Linux下复制粘贴快捷键
 1. 在终端下：

          复制命令：Ctrl + Shift + C  组合键.

          粘贴命令：Ctrl + Shift + V  组合键.

 

 2. 在控制台下：

          复制命令：Ctrl + Insert  组合键　　或　　用鼠标选中即是复制。

          粘贴命令：Shift + Insert  组合键　　或　　单击鼠标滚轮即为粘贴。
          
 
 
 # vpn链接
 帐号密码：abc014916
 高级：使用点到点加密
 网关：jp1.cetmm.cn
 # 软件安装
 sudo apt install git
 # 谷歌
 723395286@qq.com
 19910802
 
 
# [configure/make/make install的作用](http://blog.csdn.net/linzhiji/article/details/6774410)

```
这些都是典型的使用GNU的AUTOCONF和AUTOMAKE产生的程序的安装步骤。

./configure是用来检测你的安装平台的目标特征的。比如它会检测你是不是有CC或GCC，
并不是需要CC或GCC，它是个shell脚本。

make是用来编译的，它从Makefile中读取指令，然后编译。

make install是用来安装的，它也从Makefile中读取指令，安装到指定的位置。
```

# linux 下gdal的安装
```
1.下载安装包：
http://trac.osgeo.org/gdal/wiki/DownloadSource
2.解压到当前文件，进入【gdal-2.1.2】
3.执行以下代码进行编译：
  【./configure --with-python】
  【make】
  【sudo make install】
4.执行【sudo apt-get install odbcinst1debian2 libgdal1i】获取依赖的包
5.使用【python】命令进入python编译模式，使用【from osgeo import ogr】进行验证
  
```

# [linux下Linux下查看CPU型号,内存大小,硬盘空间命令](http://3lian.com/edu/2014/01-07/122036.html)
+ 查看CPU个数
># cat /proc/cpuinfo | grep "physical id" | uniq | wc -l
+ 查看CPU核数
># cat /proc/cpuinfo | grep "cpu cores" | uniq
+ 查看CPU型号
># cat /proc/cpuinfo | grep 'model name' |uniq
+ 查看内存总数
>#cat /proc/meminfo | grep MemTotal
+ 查看内存条数
># dmidecode |grep -A16 "Memory Device$"
+ 查看硬盘大小
># fdisk -l | grep Disk