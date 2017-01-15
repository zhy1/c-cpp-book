change android hosts
2017.1.5


there have meizu pro5
i see the network is dirty and horrible.
tcp/ip endless upload and download. i can't  endure.
PRO5 需要root 2次 第一次通过flyme ROOT 然后安装360Root

1. connection mobile to PC, change connection type to CD-ROM and read files,
  for add file on PC  /User/.android/adb_usb.ini
     连接到pc,修改cd-rom,添加文件

2. login flyme identify accounts and "safe and touch" for  open Root.
     登录flyme账户 然后打开root

3. download and install [ 360 root ]. allow 360 root Permission
    安装360root

4. delete about origin app
    删除原厂应用

5. change hosts : 
   download and install [ go hosts ]and import hosts file.
     [  /etc/hosts ] or [ /system/ect/hosts ]

6. close devices and boot devices -> don't just reboot. becase reboot not be reload hosts.
    关闭设备  开启设备 重启不靠谱

7. close proxy : prompt ! proxy will use remote proxy machine hosts did'nt  use local hosts.
    代理以后不会使用本地hosts

8. 本来准备退货,这下不用退货了!



[tips]



adb kill-server

adb devices

adb remount

adb root


adb shell : 进入手机根目录操作

su
ls
cd
source
echo -e \\n >> hosts
echo 127.0.0.1 u.meizu.com >> hosts
echo -e \\n >> hosts
echo 127.0.0.1 sina.cn >> hosts
cat /system/ect/hosts



documents 
https://www.zhihu.com/question/29064201

http://www.tuicool.com/articles/zAfq6bv

http://jingyan.baidu.com/article/b0b63dbfe792f94a48307090.html

mount -o rw,remount /system
chmod 0644 build.prop
http://blog.csdn.net/y22222ly/article/details/50970252

Android使用adb命令直接修改文件
http://blog.sina.com.cn/s/blog_494e45fe0102dtax.html


http://blog.csdn.net/singleton1900/article/details/18602229

android 5.1 动态hosts实现
http://blog.csdn.net/study2self/article/details/51275379


http://blog.csdn.net/sudic_niu/article/details/7676608

pro5 需要root 2次
http://bbs.meizu.cn/thread-5760011-1-1.html