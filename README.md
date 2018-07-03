# **WifiLoginer**
上海科技大学网络自动验证登录器

这里有多位同学写的不同版本，大家可以根据介绍自行选用。



----------


### **EZNetLoginer**
作者：吕文涛

环境：Linux/Mac OS X/Windows/Android/UNIX Like

语言：Python 2.5+

实现登录功能、Heartbeat保持登录、记住密码、语言切换

----------


### **WifiLoginer**
作者：陈宸

环境：Linux/Mac OS X/Windows（不建议）/UNIX Like

语言：Ruby

实现登录功能

--------


### **Shtulogin**


作者：邓岂

环境：Linux/Mac OS X/Windows etc.

语言：Golang

基本的登录功能实现

--------

### **CURL** 

作者：邓岂

环境：Linux/Mac OS X/Windows etc.

语言:shell 脚本


**需要curl**

1.命令行下直接：

```shell
curl -k -H "Content-Type: application/x-www-form-urlencoded" -X POST -v --data \
"userName=(你的用户名)&password=(你的密码)&hasValidateCode=false&authLan=zh_CN"  \
--cookie "JSESSIONID=D56359E00B58C7877668AAB44B3BFE31" \
https://controller.shanghaitech.edu.cn:8445/PortalServer//Webauth/webAuthAction\!login.action
```

2.Shell 脚本:

```
./shtech.sh 用户名 密码
```

3.用wget
wget支持下载的时候认证，所以也可以用来做认证

```shell
wget --header="Content-Type: application/x-www-form-urlencoded"  \
--no-check-certificate   \
--header="Cookie:JSESSIONID=D56359E00B58C7877668AAB44B3BFE31"    \
--post-data="userName=(用户名)&password=（密码）&hasValidateCode=false&authLan=zh_CN" \
https://controller.shanghaitech.edu.cn:8445/PortalServer//Webauth/webAuthAction\!login.action \
```
----------


### **UWPLoginer**

作者：夏寅岑

环境：Windows 10 higher than version 1511(10586)

语言：C# & XAML

实现登录功能、记住密码、后台自动登陆*

---

### **Shtulogin**

作者：邓岂

环境：Windows only. 需要 Poweshell  > 4.0.

语言：

1. 基本的登录功能
2. 保持连接
3. 账号密码的本地存储（交互式）
4. 优雅的配色

### WhyFi_Surfer （桌面窗口版）
作者：崔校友

环境：
Windows （Windows 7 or higher，需要 .net Framework 4.5）
Mac (OS X El Capitan or higher)

语言：
Windows：C#
Mac：Swift

特点：
1. 完全按照 Windows 和 macOS 的界面习惯定制的界面
2. 记住密码与定时保持连接功能

地址：
Windows：https://github.com/TomJinW/WhyFi_Surfer_Win
Mac：https://github.com/TomJinW/WhyFi_Surfer_Mac

