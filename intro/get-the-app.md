# Get the App

You can download the latest version of Anytype for your device at [download.anytype.io](https://download.anytype.io).

There is currently no [browser version](../miscellaneous/faqs.md#why-is-there-no-browser-version-of-anytype) of the app.

### Minimum specs

* For Desktop, Electron follows Chrome, and they follow [vendor support policies](https://support.google.com/chrome/a/answer/7100626?hl=en).\
  At the moment that means:
  * Win 10+
  * macOS Catalina 10.15+
  * 64-bit Ubuntu 18.04+, Debian 10+, openSUSE 15.5+, or Fedora Linux 38+
* For Android (if installed through Google Play), it's Android 8.0 and a 64-bit device with a minimum of 4GB of RAM.
* For iOS, it's iOS 16,

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

{% hint style="danger" %}
Please be cautious when using local-only mode, as your data can only be transferred to a second device via peer-to-peer (P2P) connection.
{% endhint %}

#### External drives and Cloud providers&#x20;

To store your data on an external drive, you just need to mount the drive first, and then follow the steps from [#custom-storage-location](get-the-app.md#custom-storage-location "mention").

We don't recommend using cloud providers like Google Drive or iCloud since you might end up with sync conflicts / issues.
