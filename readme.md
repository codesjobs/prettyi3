成效图：

![effect_1.png](https://i.loli.net/2020/03/19/yKBnkQZIh6YpJXL.png)

![effect_1.png](https://i.loli.net/2020/03/19/MBY2RG7TVcHZiXk.png)











本仓库fork自[prettyi3](https://github.com/aeghn/prettyi3)，对配置文件进行了部分修改。**

## 配置简介：

去除了原作者的Dark版本。

默认的mod键为Mod4，即Win键或Super键。
**本项目使用的是[i3-gaps](https://github.com/Airblader/i3)，添加的内容从343至406行为i3gaps的配置，以及417行i3bar的参数-t。此处强烈建议编译后安装i3-gaps，效果比原生的i3好多了，如果不使用i3-gaps，请注释343至406行，以及删除第417行的-t参数**

相关的应用程序有：

1.默认应用启动器为rofi，界面更美观，相关的内容在75至82行，使用Mod+o打开。

2.默认的终端为konsole，相关内容在配置文件的109行，使用Mod+Enter打开。

3.bar的工作区名称调为font-awesome（[下载地址](http://files.cnblogs.com/files/vachester/font-awesome-4.7.0.zip)），更加美观，方便辨识。下载完成解压后放到/usr/share/fonts即可（若无法使用或不愿意使用font-awesome，可以在配置文件的262行到271行进行更改）

4.使用scort为截图软件，在配置文件的91至96行调用了```~/.config/i3/screencut```里的三个脚本文件，如果不使用请删除或者注释这几行。

5.使用```compton```作为窗口透明程序，开机自动启动，相关配置在108行。

6.从112到116行是开机自动启动，软件如下，不妥的话可以进行修改。

*关于自动放置特殊应用到某一个工作区，在配置文件的299至304行，按需更改* 	

​	(1).konsole，kde的默认终端，放置于工作区1；

​	(2).Google Chorme，网页浏览器，放置于工作区2；

​	(3).Dolphin，kde的默认文件管理器，放置于工作区4。

​	(4).第114行是原作者调用的polybar，由于我无法安装polybar，对这一行进行了注释，并在下方的408行至438	行调用了i3bar。

​	(5).Feh，一个图片查看器，但此处我们使用的是它的壁纸设置功能，具体调用在第118行。默认的壁纸```~/config/i3/Pictures/wallpaper.jpg```，可以按自己的需求进行更改。

​	(6).启动了fcitx输入法。

## 关于项目的安装：

```
git clone https://github.com/voiddreamz/prettyi3.git
cd ./prettyi3/light

```
在这个文件夹下可以看到四个文件夹，Scripts复制到用户的主目录下，即```~/```

config下的所有文件夹复制到```~/.config```下

icons下的文件夹复制到```usr/share/icons```

themes下的文件夹复制到/usr/share/themes

关于gtk主题的应用，可以使用lxappearance来进行管理。

(**注意，是复制config、icons、themes下的文件夹，不是复制整个config、icons、themes文件夹**)
