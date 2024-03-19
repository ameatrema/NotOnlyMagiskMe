---
description: 各地区机器差别较大，仅供参考。
---

# 🌏 1.2.2 · 对于其他地区发售的机型

{% hint style="info" %}
**部分运营商机型可能无法解锁Bootloader。**

与国内不同，国外的部分运营商（例如美国的AT\&T、日本的docomo等）对于机器固件的控制权非常高，再加上合约等其他因素，使得很多海外机型的运营商定制版本与其共开版的Bootloader解锁政策并不相同。以下内容仅作参考，想要了解更多，请参考各品牌的详细解释，与[1.2-Ex小节](verify\_devices.md)的内容。
{% endhint %}

在这篇文章中，我们用一个稍复杂一些的表格来做一个大概的概括：

<table><thead><tr><th width="181">品牌</th><th align="center">港/澳/台</th><th align="center">美</th><th align="center">日</th><th align="center">韩</th><th align="center">欧</th></tr></thead><tbody><tr><td><a href="for_global_models.md#lg">LG</a></td><td align="center">/</td><td align="center">/</td><td align="center">/</td><td align="center">/</td><td align="center">/</td></tr><tr><td><a href="for_global_models.md#moto">moto</a></td><td align="center"><mark style="color:green;">申请</mark></td><td align="center"><mark style="color:green;">申请 *</mark></td><td align="center">/</td><td align="center">/</td><td align="center"><mark style="color:green;">申请</mark></td></tr><tr><td><a href="for_global_models.md#nothing">Nothing</a></td><td align="center"><mark style="color:green;">直接</mark></td><td align="center"><mark style="color:green;">直接</mark></td><td align="center">/</td><td align="center">/</td><td align="center"><mark style="color:green;">直接</mark></td></tr><tr><td><a href="for_global_models.md#google">Pixel</a></td><td align="center"><mark style="color:green;">直接</mark></td><td align="center"><mark style="color:green;">直接 *</mark></td><td align="center"><mark style="color:green;">直接</mark></td><td align="center">/</td><td align="center"><mark style="color:green;">直接</mark></td></tr><tr><td><a href="for_global_models.md#san-xing">三星</a></td><td align="center"><mark style="color:green;">直接</mark></td><td align="center"><mark style="color:yellow;">第三方 *</mark></td><td align="center"><mark style="color:green;">直接 *</mark></td><td align="center"><mark style="color:green;">直接</mark></td><td align="center"><mark style="color:green;">直接</mark></td></tr><tr><td><a href="for_global_models.md#suo-ni">索尼</a></td><td align="center"><mark style="color:green;">申请</mark></td><td align="center"><mark style="color:green;">申请 *</mark></td><td align="center"><mark style="color:yellow;">第三方 *</mark></td><td align="center">/</td><td align="center"><mark style="color:green;">申请</mark></td></tr><tr><td><a href="for_global_models.md#undefined">一加</a></td><td align="center"><mark style="color:green;">直接</mark></td><td align="center"><mark style="color:green;">直接 *</mark></td><td align="center">/</td><td align="center">/</td><td align="center"><mark style="color:green;">直接</mark></td></tr></tbody></table>

请注意，解锁方式后有\*标注的，表示该品牌在该地区的销售型号受运营商影响，更为详细的信息请对应至下方的详细解释。解锁方式标注/的，表示目前暂无数据，或情况过于复杂，目前尚未整理完毕，请耐心等待，欢迎反馈。

<details>

<summary>LG</summary>

**由于LG各机型可解锁情况较为复杂，且存在硬解等情况，教程仍在完善中。**目前唯一可以提供的信息是，LG已在2021.12.31关闭了官方的Bootloader解锁申请通道：

[LG Developer](https://developer.lge.com/resource/mobile/RetrieveBootloader.dev)

</details>

<details>

<summary>moto</summary>

**关于运营商的解释：**美版moto存在部分带**网络锁**的机器，无法通过正常渠道解开Bootloader锁（部分机器在原机主合约到期后即可正常解锁），对于此类机器的鉴别，请参考[1.2-Ex小节](verify\_devices.md)的内容。

对于没有网络锁的机器，若要继续，请直接移步[1.3.1小节](../ways\_to\_unlock/preparation.md)与[1.3.3小节](../ways\_to\_unlock/apply.md)，按照教程进行即可。

</details>

<details>

<summary>Nothing</summary>

若要继续，请直接移步[1.3.1小节](../ways\_to\_unlock/preparation.md)与[1.3.2小节](../ways\_to\_unlock/direct.md)，按照教程进行即可。

</details>

<details>

<summary>Pixel</summary>

**关于运营商的解释：**美版Pixel存在部分带**网络锁**的机器（又被称作“**adb解锁**”、“**OEM关**”等），无法通过正常渠道解开Bootloader锁（部分机器在原机主合约到期后即可正常解锁），对于此类机器的鉴别，请参考[1.2-Ex小节](verify\_devices.md)的内容。

对于没有网络锁的机器，若要继续，请直接移步[1.3.1小节](../ways\_to\_unlock/preparation.md)与[1.3.2小节](../ways\_to\_unlock/direct.md)，按照教程进行即可。

</details>

<details>

<summary>三星</summary>

**关于运营商的解释：**由于运营商及销售原因，即使没有运营商锁，部分美版三星机器也无法解开Bootloader，对于此类机器的鉴别，请参考[1.2-Ex小节](verify\_devices.md)的内容。

对于没有网络锁的机器，若要继续，请直接移步[1.3.1小节](../ways\_to\_unlock/preparation.md)与[1.3.2小节](../ways\_to\_unlock/direct.md)，按照教程进行即可。

</details>

<details>

<summary>索尼</summary>

**关于运营商的解释：**部分美版索尼机器由于运营商及销售原因，即使没有运营商锁，也无法解开Bootloader；而日版机器基本均为运营商定制机，绝大多数都需要通过第三方工具强制解锁。对于此类机器的鉴别，请参考[1.2-Ex小节](verify\_devices.md)的内容。

**查看能否使用申请解锁的方法：**拨号盘输入**\*#\*#7378423#\*#\***，进入**Service info > Configuration > Rooting Status**，若**Bootloader unlock allowed**后显示**Yes**，则可以使用申请解锁；若为**No**，则需要使用第三方工具，在购物平台搜索“**索尼 日版 解锁**”等关键词查找即可。

对于没有网络锁的机器，若要继续，请直接移步[1.3.1小节](../ways\_to\_unlock/preparation.md)与[1.3.3小节](../ways\_to\_unlock/apply.md)，按照教程进行即可。

</details>

<details>

<summary>一加</summary>

**关于运营商的解释：**美版一加存在部分带**网络锁**的机器，无法通过正常渠道解开Bootloader锁（部分机器在原机主合约到期后即可正常解锁），对于此类机器的鉴别，请参考[1.2-Ex小节](verify\_devices.md)的内容。

对于没有网络锁的机器，若要继续，请直接移步[1.3.1小节](../ways\_to\_unlock/preparation.md)与[1.3.2小节](../ways\_to\_unlock/direct.md)，按照教程进行即可。

</details>
