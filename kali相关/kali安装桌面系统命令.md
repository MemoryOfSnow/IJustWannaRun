# 问题1：我安装的这个kali镜像的kde plsama桌面系统的文件系统dophin在我的机器上打不开。

卸载重装
apt-get remove  kde-full
apt-get install kali-defaults kali-root-login desktop-base kde-full
解决办法：安装gnome桌面
$sudo apt-get  install gnome

若想安装Cinnamon桌面，可参考[Cinnamon桌面](https://linux.cn/article-10065-1.html)

# 问题2：缺少一些实用工具

解决办法：安装scrot截图工具，安装mplayer播放器，安装[搜狗输入法](https://pinyin.sogou.com/linux/)

# 问题3：语言和终端乱码

配置LANG：
如果你希望修改整个系统的编码和语言信息，可以修改系统的配置文件修改LANG，
而如果你不希望影响其他用户直接在你自己的~/.bashrc中配置LANG即可

## 1、安装中文语言包

sudo apt-get install language-pack-zh

## 2、用vim配置语言环境变量

vim /etc/environment

在下面添加如下两行


LANG=”zh_CN.UTF-8″

LANGUAGE=”zh_CN:zh:en_US:en”


## 2如果你想用英文环境了，改成这两行就OK


LANG=”en_US.UTF-8″

LANGUAGE=”en_US:en”
# 什么是gdm3，kdm，lightdm？如何安装和删除它们？
gdm3(gnome的)，kdm（KDE的）和lightdm（Canonical的显示管理器解决方案。它应该是轻量级的）都是显示管理员。它们提供图形登录并处理用户身份验证。
>显示管理器向用户显示登录屏幕。当用户成功输入用户名和密码的有效组合时，会话开始。
sudo apt-get install gdm3
并将其删除：
sudo apt-get remove gdm3
