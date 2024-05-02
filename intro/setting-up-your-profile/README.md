---
description: >-
  Let's get started using Anytype! Find out what you can customize in this
  chapter.
---

# 👾 Setting Up Your Vault

### Download the app

You can find the latest version of Anytype at [download.anytype.io](https://download.anytype.io).

#### Minimum specs

* For Desktop, these follow Electron who follows vendor support policies. For example, Win 7 / Win 8.1 are no longer supported.
* For Android (if installed through Google Play), it's Android 8.0 and a 64-bit device with a minimum of 4GB of RAM.
* For iOS, it's iOS 15 (soon to be iOS 16).

#### Install location

Anytype is installed:

* In Windows 10 or above, it is usually located:\
  `C:\Users\<username>\Appdata\Local\Programs\anytype2\Anytype.exe`\
  **username** stands for the name of your user aka working directory.&#x20;
* For MacOS, it's: ` HHD > Users >`` `` `_`Username`_` `` ``> Library > Application Support > anytype `
* For Linux, you'll find your work directory in `~/.config/anytype`
* For Android, it’s your default location, usually: \_device/data/app\_​.\
  We also store some caches: _device/data/data/io.anytype.app_\
  Anytype directory is stored in a protected app data folder, which isn’t accessible by the user on Android devices.
* For iOS, it's the standard install path determined by the iOS.

#### Custom Storage Location

When creating a vault, it’s now possible to select the storage location on your hard drive. If your vault has already been created, you can also change the location and retrieve the data from the network. To do so, first logout, then tap the settings wheel on the black login screen.

<figure><img src="../../.gitbook/assets/Custome Storage Location.gif" alt="" width="563"><figcaption></figcaption></figure>

Please be cautious when using local-only mode, as your data can only be transferred to a second device via peer-to-peer (P2P) connection.

{% hint style="info" %}
Anytype is a stand-alone software, that works on desktop or mobile devices. There is no browser version of the app. There are many points of vulnerability in browser apps that would compromise our commitment to data security and encryption.
{% endhint %}

### Create an account

If you haven't created an vault yet, you can easily create one by clicking **New Vault** and then following the provided instructions.

#### Log-in using your Key

On the contrary, if you already do have a vault, click on **Login** and enter your [what-is-a-recovery-phrase.md](../../data-and-security/what-is-a-recovery-phrase.md "mention") to proceed.

{% hint style="danger" %}
Make sure you store your [what-is-a-recovery-phrase.md](../../data-and-security/what-is-a-recovery-phrase.md "mention") somewhere safe, and don't ever share it with anyone who you don't trust!
{% endhint %}

#### Log-in using the QR code

In addition to using your key to log in, you can also use the QR code to login faster if your desktop is close by.

To log in using the QR code, simply navigate to your Key.

`Settings > Account > Key`.

Beneath your Key you'll find your blurred out QR code, when you click the image it will display.

Now you can scan this code with your mobile device and install the app.

### Migrate existing data

If you would like to import your existing data, you can check out [#import-and-export](space-settings.md#import-and-export "mention").
