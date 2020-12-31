# DD-windows
linux DD windows系统


说明
无限制全自动dd安装Windows
突破没有VNC,没有救援模式,内存比dd包小的限制
使用Debian Live CD中的busybox做中间媒介,经过复杂的处理使本机的网络参数传进Windows操作系统中
即使没有DHCP能够让Windows获取网络参数,也能让Windows操作系统在开机的第一时间能够连通网络
特别注意：OpenVZ构架不适用

安装运行库
#Debian/Ubuntu:
apt-get install -y xz-utils openssl gawk file

#RedHat/CentOS:
yum install -y xz openssl gawk file
如果出现错误，运行以下代码

#Debian/Ubuntu:
apt-get update

#RedHat/CentOS:
yum update
一键脚本
示例脚本，补全DD包直连地址后运行即可；

wget --no-check-certificate -qO InstallNET.sh 'https://moeclub.org/attachment/LinuxShell/InstallNET.sh' && bash InstallNET.sh -dd '[Windows dd包直连地址]'
精简版DD包
选择好版本，输入以下一键脚本即可

# DD Windows Server 2003 32位 精简版 [账户Administrator密码cxthhhhh.com]
wget --no-check-certificate -qO InstallNET.sh 'https://moeclub.org/attachment/LinuxShell/InstallNET.sh' && bash InstallNET.sh -dd 'https://oss.sunpma.com/Windows/Win_Server2003_86_Administrator_cxthhhhh.com.gz'

# DD Windows Server 2008 R2 64位 精简版 [账户Administrator密码nat.ee]
wget --no-check-certificate -qO InstallNET.sh 'https://moeclub.org/attachment/LinuxShell/InstallNET.sh' && bash InstallNET.sh -dd 'https://oss.sunpma.com/Windows/Win_Server2008R2_sp1_64_Administrator_nat.ee.gz'

# DD Windows Server 2012 R2 64位 精简版 [账户Administrator密码WinSrv2012r2x64-Chinese]
wget --no-check-certificate -qO InstallNET.sh 'https://moeclub.org/attachment/LinuxShell/InstallNET.sh' && bash InstallNET.sh -dd 'https://oss.sunpma.com/Windows/Win_Server2012R2_64_Administrator_WinSrv2012r2x64-Chinese.gz'

# DD Windows Server 2019 Datacenter 64位 精简版 [账户Administrator密码WinSrv2019dc-Chinese]
wget --no-check-certificate -qO InstallNET.sh 'https://moeclub.org/attachment/LinuxShell/InstallNET.sh' && bash InstallNET.sh -dd 'https://oss.sunpma.com/Windows/Win_Server2019_64_Administrator_WinSrv2019dc-Chinese.gz'

# DD Windows7 32位 精简版 [账户Administrator密码Windows7x86-Chinese]
wget --no-check-certificate -qO InstallNET.sh 'https://moeclub.org/attachment/LinuxShell/InstallNET.sh' && bash InstallNET.sh -dd 'https://oss.sunpma.com/Windows/Win7_86_Administrator_Windows7x86-Chinese.gz'

# DD Windows7 sp1 64位 企业精简版 [账户Administrator密码nat.ee]
wget --no-check-certificate -qO InstallNET.sh 'https://moeclub.org/attachment/LinuxShell/InstallNET.sh' && bash InstallNET.sh -dd 'https://oss.sunpma.com/Windows/Win7_sp1_64_Administrator_nat.ee.gz'

#DD Windows8.1 64位 专业精简版 [账户Administrator密码nat.ee]
wget --no-check-certificate -qO InstallNET.sh 'https://moeclub.org/attachment/LinuxShell/InstallNET.sh' && bash InstallNET.sh -dd 'https://oss.sunpma.com/Windows/Win8.1_64_Administrator_nat.ee.gz'

# DD Windows10 2019LTSC 64位 企业精简版 [账户Administrator密码nat.ee]
wget --no-check-certificate -qO InstallNET.sh 'https://moeclub.org/attachment/LinuxShell/InstallNET.sh' && bash InstallNET.sh -dd 'https://oss.sunpma.com/Windows/Win10_2019LTSC_64_Administrator_nat.ee.gz'
完整版DD包
# DD Windows Server 2012 R2 Datacenter 64位 完整版 [账户administrator密码Password147]
wget --no-check-certificate -qO InstallNET.sh 'https://moeclub.org/attachment/LinuxShell/InstallNET.sh' && bash InstallNET.sh -dd 'https://oss.sunpma.com/Windows/Whole/cn_windows2012r2_administrator_Password147.gz'

# DD Windows Server 2016 Datacenter 64位 完整版 [账户administrator密码Password147]
wget --no-check-certificate -qO InstallNET.sh 'https://moeclub.org/attachment/LinuxShell/InstallNET.sh' && bash InstallNET.sh -dd 'https://oss.sunpma.com/Windows/Whole/cn_windows2016_administrator_Password147.gz'

# DD Windows Server 2019 Datacenter 64位 完整版 [账户administrator密码Password147]
wget --no-check-certificate -qO InstallNET.sh 'https://moeclub.org/attachment/LinuxShell/InstallNET.sh' && bash InstallNET.sh -dd 'https://oss.sunpma.com/Windows/Whole/cn_windows2019_administrator_Password147.gz'

# DD Windows7 sp1 64位 [账户Administrator密码nat.ee]
wget --no-check-certificate -qO InstallNET.sh 'https://moeclub.org/attachment/LinuxShell/InstallNET.sh' && bash InstallNET.sh -dd 'https://oss.sunpma.com/Windows/Whole/Win7_sp1_64_Administrator_nat.ee.gz'

# DD Windows8.1 64位 [账户Administrator密码nat.ee]
wget --no-check-certificate -qO InstallNET.sh 'https://moeclub.org/attachment/LinuxShell/InstallNET.sh' && bash InstallNET.sh -dd 'https://oss.sunpma.com/Windows/Whole/Win8.1_64_Administrator_nat.ee.gz'

# DD Windows10 LTSC 64位 [账户Administrator密码nat.ee]
wget --no-check-certificate -qO InstallNET.sh 'https://moeclub.org/attachment/LinuxShell/InstallNET.sh' && bash InstallNET.sh -dd 'https://oss.sunpma.com/Windows/Whole/Win10_LTSC_64_Administrator_nat.ee.gz'
Oracle甲骨文
此DD包仅适用于Oracle甲骨文DD Win使用

# DD Windows7 sp1 64位 企业精简版 [账户Administrator密码nat.ee]
wget --no-check-certificate -qO InstallNET.sh 'https://moeclub.org/attachment/LinuxShell/InstallNET.sh' && bash InstallNET.sh -dd 'https://oss.sunpma.com/Windows/Oracle_Win7_sp1_64_Administrator_nat.ee.gz'

# DD Windows Server 2008 R2 64位 精简版 [账户Administrator密码nat.ee]
wget --no-check-certificate -qO InstallNET.sh 'https://moeclub.org/attachment/LinuxShell/InstallNET.sh' && bash InstallNET.sh -dd 'https://oss.sunpma.com/Windows/Oracle_Win_Server2008R2_sp1_64_Administrator_nat.ee.gz'
OVH
此DD包仅适用于OVH云服务器DD Win使用
说明：OVH需要使用网络参数进行安装，需要的可以参考下面的安装方法，博主并未进行测试，这里仅提供直链包；

# DD Windows7 64位 精简版 [账户administrator密码www.80host.com]
https://oss.sunpma.com/Windows/win/OVH_Win7_64_administrator_www.80host.com.gz
网络参数安装
比如GCP谷歌云Azure微软云OVH云服务器等需要指定网络参数安装的方式，示例为GCP谷歌云

# 将X.X.X.X替换为自己的网络参数.
# --ip-addr :IP Address/内网IP地址
# --ip-mask :Netmask   /子网掩码
# --ip-gate :Gateway   /网关
wget --no-check-certificate -qO InstallNET.sh 'https://moeclub.org/attachment/LinuxShell/InstallNET.sh' && bash InstallNET.sh --ip-addr X.X.X.X --ip-mask X.X.X.X --ip-gate X.X.X.X -dd 'DD包 直链地址'
例：
替换--ip-addr后面的X.X.X.X为你自己的内网IP即可；
在GCP谷歌云 Debian / Ubuntu 测试成功， CentOS 未测试；
账户：Administrator 密码：nat.ee
GCP谷歌云 香港

wget --no-check-certificate -qO InstallNET.sh 'https://moeclub.org/attachment/LinuxShell/InstallNET.sh' && bash InstallNET.sh --ip-addr X.X.X.X --ip-mask 255.255.255.0 --ip-gate 10.170.0.1 -dd 'https://oss.sunpma.com/Windows/Win7_sp1_64_Administrator_nat.ee.gz'
GCP谷歌云-台湾

wget --no-check-certificate -qO InstallNET.sh 'https://moeclub.org/attachment/LinuxShell/InstallNET.sh' && bash InstallNET.sh --ip-addr X.X.X.X --ip-mask 255.255.255.0 --ip-gate 10.140.0.1 -dd 'https://oss.sunpma.com/Windows/Win7_sp1_64_Administrator_nat.ee.gz'
连接上后如果遇到无法打开网页的情况，修改DNS即可

8.8.8.8
8.8.4.4
关于激活
可以使用本博客的KMS激活

如果不能使用KMS激活，可以试试下面的Key（不一定都能成功激活）

# Windows 7 企业版
KMS密钥：33PXH-7Y6KF-2VJC9-XBBR8-HVTHH / RHTBY-VWY6D-QJRJ9-JGQ3X-Q2289 / H8PDJ-H4NKW-3GKH7-YHKJ7-4C2JR

# Windows 8.1 专业版
KMS密钥：GCRJD-8NW9H-F2CDX-CCM8D-9D6T9

# Windows 10 LTSC 2019 企业版
KMS密钥：M7XTQ-FN8P6-TTKYV-9D4CC-J462D

# Windows Server 2019 数据中心版
KMS密钥：WMDGN-G9PQG-XVVXX-R3X43-63DFG
右键以管理员身份运行CMD（命令提示符），依次执行下面的命令；

slmgr.vbs -upk
slmgr.vbs -ipk KMS密钥
slmgr.vbs -ato
slmgr.vbs -dlv
Windows 7 旗舰版可能无法使用KMS进行激活，可以使用以下工具永久激活
激活工具：https://sunpma.lanzous.com/i0ohrjljzwb

Windows服务器开启Ping功能，打开系统运行服务 Win+R 输入命令

## 开启Ping ##
netsh firewall set icmpsetting 8
## 关闭Ping ##
netsh firewall set icmpsetting 8 disable
备用链接
百度网盘
链接：https://pan.baidu.com/s/1afwD0Is8MrvSiL8wkjoXhA
提取码：qynd
