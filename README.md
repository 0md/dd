# �ȿ����е�һ��DD�ű�

## ע��:
ȫ�Զ���װĬ��root����:``` Vicer ```,��װ��ɺ���������������.

�ܹ�ȫ�Զ���װDebian/Ubuntu/CentOS��ϵͳ.

ͬʱ�ṩdd��װ������,����: ȫ�Զ��޾�Ԯdd��װwindowsϵͳ

ȫ�Զ���װCentOSʱĬ���ṩVNC����,��ʹ��VNC Viewer�鿴����,

VNC�˿�Ϊ``` 1``` ����``` 5901``` ,�����г�������.(�ɹ���VNC���ܻ���ʧ.)

ĿǰCentOSϵͳֻ֧������汾��װΪ CentOS 6.x �����°汾.

�ر�ע��:OpenVZ���ܲ�����.


## ȷ����װ���������:

``` 
#Debian/Ubuntu:
apt-get install -y xz-utils openssl gawk file
 
#RedHat/CentOS:
yum install -y xz openssl gawk file
``` 

## ��������˴���,������:
``` 
#Debian/Ubuntu:
apt-get update
 
#RedHat/CentOS:
yum update
``` 

## ����ʹ��ʾ��:
``` 	
bash <(wget --no-check-certificate -qO- 'https://raw.githubusercontent.com/veip007/InstallNET.sh') -d 8 -v 64 -a
``` 

## ���ؼ�˵��:
``` 
wget --no-check-certificate -qO InstallNET.sh 'https://raw.githubusercontent.com/veip007/InstallNET.sh' && chmod a+x InstallNET.sh
``` 
```
Usage:
        bash InstallNET.sh      -d/--debian [dist-name]
                                -u/--ubuntu [dist-name]
                                -c/--centos [dist-version]
                                -v/--ver [32/i386|64/amd64]
                                --ip-addr/--ip-gate/--ip-mask
                                -apt/-yum/--mirror
                                -dd/--image
                                -a/-m
 
# dist-name: ���а汾����
# dist-version: ���а汾��
# -apt/-yum/--mirror : ʹ�ö��徵��
# -a/-m : ѯ���Ƿ��ܽ���VNC���в���. -a Ϊ����ʾ(һ������ȫ�Զ���װ), -m Ϊ��ʾ.
```

## ʹ��ʾ��:
```
#ʹ��Ĭ�Ͼ���ȫ�Զ���װ
bash InstallNET.sh -d 8 -v 64 -a
 
#ʹ���Զ��徵��ȫ�Զ���װ
bash InstallNET.sh -c 6.9 -v 64 -a --mirror 'http://mirror.centos.org/centos'
 
 
# ����ʾ����,��X.X.X.X�滻Ϊ�Լ����������.
# --ip-addr :IP Address/IP��ַ
# --ip-gate :Gateway   /����
# --ip-mask :Netmask   /��������
 
#ʹ���Զ��徵���Զ����������ȫ�Զ���װ
#bash InstallNET.sh -u 16.04 -v 64 -a --ip-addr x.x.x.x --ip-gate x.x.x.x --ip-mask x.x.x.x --mirror 'http://archive.ubuntu.com/ubuntu'
 
#ʹ���Զ����������ȫ�Զ�dd��ʽ��װ
#bash InstallNET.sh --ip-addr x.x.x.x --ip-gate x.x.x.x --ip-mask x.x.x.x -dd 'https://moeclub.org/get-win7embx86-auto'
 
#ʹ���Զ����������ȫ�Զ�dd��ʽ��װ�洢�ڹȸ������еľ���(�����ļ�ID�ķ�ʽ)
#bash InstallNET.sh --ip-addr x.x.x.x --ip-gate x.x.x.x --ip-mask x.x.x.x -dd "$(echo "1cqVl2wSGx92UTdhOxU9pW3wJgmvZMT_J" |xargs -n1 bash <(wget --no-check-certificate -qO- 'https://moeclub.org/get-gdlink'))"
 
#ʹ���Զ����������ȫ�Զ�dd��ʽ��װ�洢�ڹȸ������еľ���
#bash InstallNET.sh --ip-addr x.x.x.x --ip-gate x.x.x.x --ip-mask x.x.x.x -dd "$(echo "https://drive.google.com/open?id=1cqVl2wSGx92UTdhOxU9pW3wJgmvZMT_J" |xargs -n1 bash <(wget --no-check-certificate -qO- 'https://moeclub.org/get-gdlink'))"
```

## һЩ���þ����ַ:
```
# �Ƽ�ʹ�ô��� /GoogleDrive/<File_ID> ����, �ٶȸ���.
# ��ȻҲ����ʹ���Լ�GoogleDrive�д���ľ���,ʹ�÷�ʽ:
  https://image.moeclub.org/GoogleDrive/<File_ID>
 
# win7emb_x86.tar.gz:
  https://image.moeclub.org/GoogleDrive/1srhylymTjYS-Ky8uLw4R6LCWfAo1F3s7 
  https://image.moeclub.org/win7emb_x86.tar.gz
 
# win8.1emb_x64.tar.gz:
  https://image.moeclub.org/GoogleDrive/1cqVl2wSGx92UTdhOxU9pW3wJgmvZMT_J
  https://image.moeclub.org/win8.1emb_x64.tar.gz
```

## һЩ��ʾ:

�ر�ע��:

�ȿ��ṩ��dd��װ����

Զ�̵�½�˺�Ϊ: ```Administrator```

Զ�̵�½����Ϊ: ```Vicer```

���޸���������,�ɷ���ʹ��.(�����Լ�����.)

��dd��װϵͳ����ʱ:

����Ļ�����ȫ�°�װ,�������VNC,���Կ���ȫ������.

��dd��װ����Ĺ�����,�����߽�����(������һֱ��ʾΪ0%).��ɺ󽫻��Զ�����.

�����������һ����ʾΪ: ��Starting up the partitioner��

ʹ�ùȸ������д���ľ���: [�����ƴ�С] ��ȡ�ȸ������ļ���ʱֱ����������

��ȫ�Զ���װCentOSʱ:

������� ��Starting graphical installation�� �������Ʊ��,���ʾ���ڰ�װ.

���������ֻ��Ҫ���ĵȴ���װ��ɼ���.

�����Ҫ�鿴����,ʹ��VNC Viewer(��������VNC���ӹ���)

������ʾ�е�IP��ַ:�˿ڽ�������.(�˿�һ��Ϊ```1```����```5901```)



ת�����ȿ�https://moeclub.org/2018/04/03/603/