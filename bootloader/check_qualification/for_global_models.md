---
description: 各地区机器差别较大，仅供参考。
---

# 🌏 1.2.2 · 对于其他地区发售的机型

{% hint style="info" %}
**部分运营商机型可能无法解锁Bootloader。**

与国内不同，国外的部分运营商（例如美国的AT\&T、日本的docomo等）对于机器固件的控制权非常高，再加上合约等其他因素，使得很多海外机型的运营商定制版本与其共开版的Bootloader解锁政策并不相同。以下内容仅作参考，想要了解更多，请参考各品牌的详细解释，与[1.2-Ex小节](verify\_devices.md)的内容。
{% endhint %}

在这篇文章中，我们用一个稍复杂一些的表格来做一个大概的概括：

| 品牌                                              |                 港/澳/台                |                     美                     |                     日                     |                   韩                  |                   欧                  |
| ----------------------------------------------- | :----------------------------------: | :---------------------------------------: | :---------------------------------------: | :----------------------------------: | :----------------------------------: |
| [Google (Pixel)](for\_global\_models.md#google) | <mark style="color:green;">直接</mark> |  <mark style="color:green;">直接 \*</mark>  |    <mark style="color:green;">直接</mark>   |                   /                  | <mark style="color:green;">直接</mark> |
| [LG](for\_global\_models.md#lg)                 |                   /                  |                     /                     |                     /                     |                   /                  |                   /                  |
| [moto](for\_global\_models.md#moto)             | <mark style="color:green;">申请</mark> |  <mark style="color:green;">申请 \*</mark>  |                     /                     |                   /                  | <mark style="color:green;">申请</mark> |
| [Nothing](for\_global\_models.md#nothing)       | <mark style="color:green;">直接</mark> |    <mark style="color:green;">直接</mark>   |                     /                     |                   /                  | <mark style="color:green;">直接</mark> |
| [三星](for\_global\_models.md#san-xing)           | <mark style="color:green;">直接</mark> | <mark style="color:yellow;">第三方 \*</mark> |  <mark style="color:green;">直接 \*</mark>  | <mark style="color:green;">直接</mark> | <mark style="color:green;">直接</mark> |
| [索尼](for\_global\_models.md#suo-ni)             | <mark style="color:green;">申请</mark> |  <mark style="color:green;">申请 \*</mark>  | <mark style="color:yellow;">第三方 \*</mark> |                   /                  | <mark style="color:green;">申请</mark> |
| [一加](for\_global\_models.md#undefined)          | <mark style="color:green;">直接</mark> |  <mark style="color:green;">直接 \*</mark>  |                     /                     |                   /                  | <mark style="color:green;">直接</mark> |

请注意，解锁方式后有\*标注的，表示该品牌在该地区的销售型号受运营商影响，更为详细的信息请对应至下方的详细解释。解锁方式标注/的，表示目前暂无数据，或情况过于复杂，目前尚未整理完毕，请耐心等待，欢迎反馈。

<details>

<summary>Google (Pixel)</summary>

**关于运营商的解释：**美版Pixel存在部分带**网络锁**的机器（又被称作“**adb解锁**”、“**OEM关**”等），无法通过正常渠道解开Bootloader锁（部分机器在原机主合约到期后即可正常解锁），对于此类机器的鉴别，请参考[1.2-Ex小节](verify\_devices.md)的内容。

对于没有网络锁的机器，若要继续，请直接移步[1.3.1小节](../ways\_to\_unlock/preparation.md)与[1.3.2小节](../ways\_to\_unlock/direct.md)，按照教程进行即可。

</details>

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

<summary>三星</summary>

**关于运营商的解释：**由于运营商及销售原因，即使没有运营商锁，部分美版三星机器也无法解开Bootloader，对于此类机器的鉴别，请参考[1.2-Ex小节](verify\_devices.md)的内容。

对于没有网络锁的机器，若要继续，请直接移步[1.3.1小节](../ways\_to\_unlock/preparation.md)与[1.3.2小节](../ways\_to\_unlock/direct.md)，按照教程进行即可。

</details>

<details>

<summary>索尼</summary>

**关于运营商的解释：**部分美版索尼机器由于运营商及销售原因，即使没有运营商锁，也无法解开Bootloader；而日版机器基本均为运营商定制机，绝大多数都需要通过第三方工具强制解锁。对于此类机器的鉴别，请参考[1.2-Ex小节](verify\_devices.md)的内容。

日版机器查看能否使用申请解锁的方法：

对于没有网络锁的机器，若要继续，请直接移步[1.3.1小节](../ways\_to\_unlock/preparation.md)与[1.3.3小节](../ways\_to\_unlock/apply.md)，按照教程进行即可。

</details>

<details>

<summary>一加</summary>

**关于运营商的解释：**美版一加存在部分带**网络锁**的机器，无法通过正常渠道解开Bootloader锁（部分机器在原机主合约到期后即可正常解锁），对于此类机器的鉴别，请参考[1.2-Ex小节](verify\_devices.md)的内容。

对于没有网络锁的机器，若要继续，请直接移步[1.3.1小节](../ways\_to\_unlock/preparation.md)与[1.3.2小节](../ways\_to\_unlock/direct.md)，按照教程进行即可。

</details>

