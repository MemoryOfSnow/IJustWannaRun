# Linux����ָ����2000������ά��ָ����Ҫ��ס50~70����
**���±��뱻��ס�Ĺؼ��֣�**

- more ��ҳ�鿴�ļ�����
  - �ո� ���·�ҳ��b���Ϸ�ҳ��q����Ԥ��
- less
- head
- tail
- grep
- du
 - ͳ��Ŀ¼���� du -sh /etc
- wc
 - wc -l ͳ���ļ��ж�����
- alias ����ʱ��3�ַ�ʽ
 - 1.�ڵ�ǰ�ն�
 - 2. �ڵ�ǰ�û��ļ�Ŀ¼
 ```bash
 cat ~/.bashrc
 source ~/.bashrc
```
 - ���������û�����
 ```bash
 /etc/bashrc
```
- find���������ң������������ã�
���ڹܵ���֧�ַǳ�����
```bash
find /etc/ -size +1M -exec ls -lh {} \;
```
---
```bash
uname -r
uname -a
free -m
#Mem:�����ڴ�
#Swap�������ڴ�
cat etc/proc/userinfo
#lm ֧��64λ,vmx֧�����⻯
cat /etc/redhat-release
#��������汾
systemctl poweroff
poweroff /init 0/shutdown /halt
###
systemctl reboot
/boot��Linux�ܲ���������������ļ���ά����
/etc��ҳ�濨ס�������ļ��С�
/var��ҵ�����ݴ��Ŀ¼��
###���������ļ����뱸�ݡ�
/home����ͨ�û���Ŀ¼��
/mnt�����̵Ĺ���ʹ��
|  ,��ʾ��ǰһ��ָ��������������һ��ָ���������ʹ�á�
Ctrl+L������<=>clear
Ctrl+A,Ctrl+E�����ǰ�����
touch�����հ��ļ�
lm -li
rm -rf
```
