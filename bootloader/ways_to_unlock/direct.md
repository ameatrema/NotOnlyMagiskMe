---
description: 数据无价，注意备份。
---

# 🔓 1.3.2 · 直接解锁

{% hint style="danger" %}
**解锁后所有数据都会被抹除，请先备份数据再解锁**

为了保证数据的可靠性，在执行Bootloader解锁操作后，手机会被恢复至出厂状态，任何自己存储的数据，如安装的应用程序、手机上存储的各类媒体文件等，都会被清除，且无法恢复。

因此，在解锁前，请使用官方的备份软件或云同步服务，将重要数据备份至电脑、U盘、或云盘等其他地方，确保重要数据都已经转移后，再执行解锁操作。官方提供的服务可在设置中搜索“备份”“云服务”等字样进行查找。
{% endhint %}

{% hint style="danger" %}
**若手机已经登录了Google账号，请提前退出登录**

**若手机已经登录了厂商账号（如小米账号），请确保您知道密码，或提前退出登录**

部分机型即使在抹除数据后，其存储的Google账户信息仍然会保存在手机中**（尤其是海外发售的机型）**。由于解锁Bootloader会抹除数据，如果没有提前退出登录，为排除设备遭到盗窃的可能性，系统将会要求您登录之前的Google账号后，才能继续设置。由于特殊的上网环境，该步骤在国内较难进行。除非您有办法可以让手机正确访问Google服务，否则请先退出登录后，再进行下面的操作。

部分机型即使在抹除数据后，其存储的账户信息仍然会保存在手机中（如小米、OPPO、vivo等）。由于解锁Bootloader会抹除数据，如果没有提前退出登录，且开启了手机的查找功能，系统将会要求您登录之前的账号后，才能继续设置。若您已经忘记了登陆密码，请及时使用“忘记密码”等功能进行重置，并退出登录后，再进行下面的操作。
{% endhint %}

{% hint style="info" %}
**该部分教程以Windows系统为例，且推荐使用Windows 10及更高版本。**
{% endhint %}

### 一、手机上的准备：进入Bootloader

在开始解锁前，我们需要先进入手机的Bootloader。在这里，有两种方法可以进入：

#### 方法1：使用手机按键进入

* 确认手机已经按[1.3.1小节](preparation.md)中的内容设置完毕，即**电脑可以正常识别设备**
* 断开电脑与手机的连接，将手机**关机，并等待20秒左右，确保手机已完全关闭**
* 对大部分机型来说，**同时按住电源键与音量下键**，并**保持几秒**
* 此时手机可能会显示诸如**“FASTBOOT”**、**“Fastboot Mode”**，或**下载图标**等内容，表明手机已经进入了Bootloader**（如果手机没有反应，或出现了其他内容，请查看下方的说明）**

{% hint style="info" %}
**各机型进入Bootloader的组合键可能会有差异。**

部分机型进入Bootloader的按键与其他机型可能有差异。如三星机型为**音量上+音量下**等。若在尝试教程所给的所有按键组合后，仍然无法正常进入Bootloader，请搜索`具体手机型号+进入Bootloader`。
{% endhint %}

{% hint style="warning" %}
**若手机出现了无法理解的画面，请尝试强制重启。**

若教程提供的进入方法与大家的手机不匹配，可能会使设备进入其他模式，如恢复模式（Recovery）等。若无法理解手机上显示的画面，请尝试长按电源键强制重启设备。

请注意，**长按电源键的时间可能会非常长，甚至超过30秒**。若仍无法重启，请搜索`具体型号+强制重启`或联系手机售后服务。
{% endhint %}

#### 方法2：使用电脑adb进入

* 确认手机已经按[1.3.1小节](preparation.md)中的内容设置完毕，即**电脑可以正常识别设备**
* 保持手机与电脑的连接状态，在cmd中输入`adb reboot bootloader`
* 此时手机会自动重启，并显示诸如**“FASTBOOT”**、**“Fastboot Mode”**，或**下载图标**等内容，表明手机已经进入了Bootloader

### 二、电脑上的准备：使用adb进行操作

#### 1. 确认手机与电脑已正确连接

在手机成功进入Bootloader模式后，就可以进行进一步操作了：

* 将手机连接至电脑
* 在`platform-tools`文件夹中启动cmd
* 在cmd中输入`fastboot devices`

此时，你应该会在cmd中看到以下内容：

```
List of devices attached 
XXXXXXXX fastboot
```

其中，`XXXXXXXX`指代了设备的标识符，每个设备都不同。若标识符后显示`unauthorized`或其他内容，甚至在输入`fastboot devices`后没有出现任何内容，请再次查看并尝试[1.3.1小节](preparation.md)有关“连接不成功的疑难解答”中的相关解决方案。

#### 2. 解锁Bootloader

在连接成功后，就可以进行进一步操作了：

* 在cmd中输入`fastboot oem unlock`
* 此时手机界面会显示警告信息，按下手机音量键，使`Unlock the Bootloader`选项被选中，随后按下电源键确认
* 此时手机会自动重启几次，完成清除数据操作，并进入开机向导

至此，手机的Bootloader就已经解除，可以进行下一步——刷入Magisk了：

{% content-ref url="../../flash_magisk/how_to_flash.md" %}
[how\_to\_flash.md](../../flash\_magisk/how\_to\_flash.md)
{% endcontent-ref %}

{% hint style="info" %}
**手机在解锁Bootloader后，每次开机时均会显示警告信息。**

在解锁Bootloader后，每次开机时，都会显示一些警告信息，如：

<mark style="color:orange;">`<!>`</mark>

`The boot loader is unlocked and software integrity cannot be guaranteed. Any data stored on the device may be available to attackers. Do not store any sensitive data on the device.`

`Visit this link on another device:`

<mark style="color:orange;">`g.co/ABH`</mark>

`PRESS POWER KEY TO PAUSE BOOT`

这是正常现象，忽略即可。若无法接受，请考虑查看[1.3-Ex小节](ways\_to\_lock.md)的相关内容来回锁Bootloader。


{% endhint %}
