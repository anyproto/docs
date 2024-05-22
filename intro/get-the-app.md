# Get the App

You can download the latest version of Anytype for your device at [download.anytype.io](https://download.anytype.io).

{% hint style="info" %}
Anytype is a stand-alone software, that works on desktop or mobile devices. There is no browser version of the app. There are many points of vulnerability in browser apps that would compromise our commitment to data security and encryption.
{% endhint %}

### Minimum specs

* For Desktop, we follow Electron who follows vendor support policies. For example, Win 7 / Win 8.1 are no longer supported because Microsoft no longer supports them either.
* For Android (if installed through Google Play), it's Android 8.0 and a 64-bit device with a minimum of 4GB of RAM.
* For iOS, it's iOS 15 (soon to be iOS 16).

### Install location

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

### Custom Storage Location

When creating a Vault, it’s now possible to select the storage location on your hard drive. If your Vault has already been created, you can also change the location and retrieve the data from the network. To do so, first logout, then tap the settings wheel on the black login screen.

<figure><img src="../.gitbook/assets/Custome Storage Location.gif" alt="" width="563"><figcaption></figcaption></figure>

Please be cautious when using local-only mode, as your data can only be transferred to a second device via peer-to-peer (P2P) connection.
