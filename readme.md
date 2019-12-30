#安卓刷机教程
##手机：google pixel

##版本：andorid 7.1.2

### 包和安装过程可能会因为手机和android版本而大同小异

1.安装adb和fastboot，这两个工具在android sdk platform-tools中

2.下载SuperSU.zip,网址：https://supersuroot.org/

3.下载twrp.img，网址：https://dl.twrp.me/(根据手机型号要下载对应的版本)

4.用adb push 命令将SuperSU.zip拷贝到手机sdcard下面

5.adb reboot bootloader让手机进入booeloader模式

6.fastboot oem unlock,会提示解锁成功，界面显示start

7.重启手机，继续adb reboot bootloader

8.用音量加减键选择recovery模式fastboot boot twrp.XXXX.img

9.成功后会自动进入twrp， 在settings把promt install twrp的选项勾掉， 进入install选项点击SuperSU.zip滑动安装

10.提示成功后选择reboot system，重启后会发现多了SuperSU标志

11.adb shell，输入su，SuperSU会提示授权，成功
