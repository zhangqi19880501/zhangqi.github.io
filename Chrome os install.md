# (推荐一个我自己做的普法公众号，[大可说法律](http://mp.weixin.qq.com/s?__biz=MzkwMDE5NzAyNw==&mid=2247483793&idx=1&sn=4b67d0bbaceb57eabf7403cdfb138b02&chksm=c046fe5df731774b3f92a562c2c05499f9b3203e8ebe1beb5349eb463da64b9ca7042296c28a&token=869479509&lang=zh_CN#rd)，有法律方面咨询的可以关注)
# 文件下载
链接：https://pan.baidu.com/s/1dWWeOooEoF0hFHWBdjulKg 
提取码：u4n7 

- 1 ubuntu-mate-20.04.2.0-desktop-amd64.iso
- 2 Rufus_3.13.1730.0.exe
- 3 brunch_r88_stable_20210223.tar.gz
- 4 chromeos_13505.111.0_rammus_recovery_stable-channel_mp-v2.bin.zip 

# 备用命令：
install.sh脚本命令：

```
sudo apt-get update
sudo apt-get install figlet
sudo apt-get install pv
sudo apt-get install cgpt
sudo bash chromeos-install.sh -src rammus_recovery.bin -dst /dev/sda
```
文件下载完毕后，安装Rufus，将ubuntu-mate-20.04.2.0-desktop-amd64.iso写入**16G优盘**（分区类型选择**GPT**，目标系统类型：**uefi**）。
![在这里插入图片描述](https://img-blog.csdnimg.cn/20210318150805286.png)

然后在制作好的u盘内新建文件夹：Chrome OS。
解压brunch_r88_stable_20210223文件，到Chrome OS。

解压 chromeos_13505.111.0_rammus_recovery_stable-channel_mp-v2.bin.zip到 Chrome OS，并修改文件名为：rammus_recovery.bin。
此时Chrome OS文件夹内应当为图中所示。

u盘插入电脑，像安装Ubuntu系统一样，试用ubuntu就好了。进入后，设置连接谷歌的网络。你懂的。*无法联网的朋友请撤退。*

![在这里插入图片描述](https://img-blog.csdnimg.cn/20210318154139538.png?x-oss-process=image/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L3FxXzQzMjAyOTUz,size_16,color_FFFFFF,t_70)

进入到file system -> cdrom-> Chrome OS， 打开命令终端，输入上述命令：

```
sudo apt-get update
sudo apt-get install figlet
sudo apt-get install pv
sudo apt-get install cgpt
sudo bash chromeos-install.sh -src rammus_recovery.bin -dst /dev/sda
```
安装时候询问是否清空硬盘，输入yes然后等待。重启完毕。
