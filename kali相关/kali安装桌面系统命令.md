# ����1���Ұ�װ�����kali�����kde plsama����ϵͳ���ļ�ϵͳdophin���ҵĻ����ϴ򲻿���

ж����װ
apt-get remove  kde-full
apt-get install kali-defaults kali-root-login desktop-base kde-full
����취����װgnome����
$sudo apt-get  install gnome

���밲װCinnamon���棬�ɲο�[Cinnamon����](https://linux.cn/article-10065-1.html)

# ����2��ȱ��һЩʵ�ù���

����취����װscrot��ͼ���ߣ���װmplayer����������װ[�ѹ����뷨](https://pinyin.sogou.com/linux/)

# ����3�����Ժ��ն�����

����LANG��
�����ϣ���޸�����ϵͳ�ı����������Ϣ�������޸�ϵͳ�������ļ��޸�LANG��
������㲻ϣ��Ӱ�������û�ֱ�������Լ���~/.bashrc������LANG����

## 1����װ�������԰�

sudo apt-get install language-pack-zh

## 2����vim�������Ի�������

vim /etc/environment

�����������������


LANG=��zh_CN.UTF-8��

LANGUAGE=��zh_CN:zh:en_US:en��


## 2���������Ӣ�Ļ����ˣ��ĳ������о�OK


LANG=��en_US.UTF-8��

LANGUAGE=��en_US:en��
# ʲô��gdm3��kdm��lightdm����ΰ�װ��ɾ�����ǣ�
gdm3(gnome��)��kdm��KDE�ģ���lightdm��Canonical����ʾ�����������������Ӧ�����������ģ�������ʾ����Ա�������ṩͼ�ε�¼�������û������֤��
>��ʾ���������û���ʾ��¼��Ļ�����û��ɹ������û������������Ч���ʱ���Ự��ʼ��
sudo apt-get install gdm3
������ɾ����
sudo apt-get remove gdm3
