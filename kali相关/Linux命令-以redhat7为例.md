# Linux常见指令有2000当个；维护指令大概要记住50~70个。
**本章必须被记住的关键字：**

- more 分页查看文件内容
  - 空格 向下翻页，b向上翻页，q结束预览
- less
- head
- tail
- grep
- du
 - 统计目录内容 du -sh /etc
- wc
 - wc -l 统计文件有多少行
- alias 建立时有3种方式
 - 1.在当前终端
 - 2. 在当前用户的家目录
 ```bash
 cat ~/.bashrc
 source ~/.bashrc
```
 - 对于所有用户可用
 ```bash
 /etc/bashrc
```
- find（立即查找，生产环境慎用）
对于管道的支持非常弱。
```bash
find /etc/ -size +1M -exec ls -lh {} \;
```
---
```bash
uname -r
uname -a
free -m
#Mem:固有内存
#Swap：虚拟内存
cat etc/proc/userinfo
#lm 支持64位,vmx支持虚拟化
cat /etc/redhat-release
#获得主机版本
systemctl poweroff
poweroff /init 0/shutdown /halt
###
systemctl reboot
/boot，Linux能不能启动都看这个文件的维护。
/etc，页面卡住，配置文件夹。
/var，业务数据存放目录。
###以上三个文件必须备份。
/home，普通用户家目录。
/mnt，磁盘的挂载使用
|  ,表示将前一个指令的输出，当作下一个指令的输入来使用。
Ctrl+L清屏，<=>clear
Ctrl+A,Ctrl+E光标最前和最后
touch创建空白文件
lm -li
rm -rf
```
