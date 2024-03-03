---
description: Instructions for our Alpha testers
---

# 从旧版应用（Legacy）迁移

#### **如何迁移？**

如果你已在 Alpha/Legacy 版本（0.31.\* 及更早版本）中创建了想要保留的内容，则需要对其进行迁移。这个过程相对比较简单：

1. 通过 Anytype > 检查更新，或通过 [这个链接](https://download.anytype.io/?ref=migration\&platform=desktop)，将桌面端的旧版应用程序更新到其最新版本 (0.31.9)。

<div align="left">

<figure><img src="../../.gitbook/assets/Check updates.png" alt="" width="331"><figcaption></figcaption></figure>

</div>
2. 从更新后的旧版应用程序导出：文件 > 导出 > Protobuf。

<div align="left">

<figure><img src="../../.gitbook/assets/Anytype Export.gif" alt="" width="336"><figcaption></figcaption></figure>

</div>
3. [下载](https://download.anytype.io/)，安装，并打开 Beta 版应用。
4. 将你的备份导入 Beta 版应用。

有关更多详细信息，请查看我们的 [迁移路径指南](https://community.anytype.io/t/anytype-legacy-to-beta-migration-trail-guide/9274)。

#### **在哪里下载最新的 Alpha （旧版）应用程序**

如果你在导出数据前已经删除了 Alpha 应用程序，则可能需要重新下载它来完成导出。你可以通过 [以下链接](https://download.anytype.io/?ref=migration\&platform=desktop) 下载适用于 Mac、Windows 和 Linux 版的 0.31.9 桌面端应用程序。

#### 我怎样跳过导入备份步骤？

除了迁移，你还有以下选择：

* 创建新账户。启动应用程序时，选择“注册”(Join) 而不是“登录”(Login)。

<div align="left">

<figure><img src="../../.gitbook/assets/Join Anytype.png" alt="" width="354"><figcaption></figcaption></figure>

</div>
* 将选择的【对象】逐个从 Legacy 版手动导入到 Beta 版。如果你的 Legacy 帐户已经变得乱七八糟，但你有一些项目想转到 Beta 版，可能需要这样做。

对于这些选择，你都需要创建一个新账户，这将生成一个新的【恢复短语】。

#### 故障排除

* 错误“open profile: file does not exist”
   * 原因：旧的 Legacy 版本（如 0.31.0）会出现这种情况。
   * 解决方法：按上述说明更新 Legacy 版应用程序。
* 错误“无法运行服务 'client.clientspace'：EOF”\*
