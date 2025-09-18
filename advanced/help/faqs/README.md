# FAQs

<details>

<summary>How to recover my Key from my OS key storage manager?</summary>

#### Mac

If you’re using a Mac, Anytype’s default setting is to store your key in the native Keychain Access app. It doesn’t get stored anywhere else. Whether your passwords are backed up to iCloud depends if you have that option enabled in your settings. You can check [Apple’s support page](https://support.apple.com/en-us/HT204085) for more information on iCloud password backups.

We’ve set up this system as a safety net for users who might otherwise lose their Key. We’re pursuing different options for the future, but for the time being, this is how it works.

If you logged in with your key on your mac, then you can find it here:

1. Click and open Finder from the dock.
2. Click on Applications & open Utilities.
3. Open the Keychain Access app.
4. On the sidebar: select Default Keychains: login
5. Find & open your Anytype instance in the list
6. Check the “Show password” box to reveal your key

#### Windows

Your key is stored in the [Credentials Manager](https://support.microsoft.com/en-us/windows/accessing-credential-manager-1b5c916a-6a16-889f-8581-fc16e8165ac0). If you are unable to read a password via the Credential Manager (Show button is missing), you can use [this PowerShell script](https://gist.github.com/requilence/de8da32adc44d4786559789debb3bf88). Save it to your computer, right-click in the File Explorer and press "Run with PowerShell".

#### Linux

You can use [seahorse](https://wiki.gnome.org/Apps/Seahorse/) to find your key if you are using [GNOME Keyring](https://wiki.gnome.org/action/show/Projects/GnomeKeyring?action=show\&redirect=GnomeKeyring).

</details>

<details>

<summary>Which standard do you follow to create my Vault’s Key?</summary>

We use the [**BIP39**](https://medium.com/coinmonks/mnemonic-generation-bip39-simply-explained-e9ac18db9477) standard to generate a mnemonic phrase, which is then used to derive your Vault's private key.

</details>

<details>

<summary>What are the minimum specs?</summary>

* For Desktop, Electron follows Chrome, and they follow [vendor support policies](https://support.google.com/chrome/a/answer/7100626?hl=en).\
  At the moment that means:
  * Win 10+
  * macOS 12 Monterey and up
  * 64-bit Ubuntu 18.04+, Debian 10+, openSUSE 15.5+, or Fedora Linux 39+
* For Android (if installed through Google Play), it's Android 8.0 and a 64-bit device with a minimum of 4GB of RAM.
* For iOS, it's iOS 16.

</details>

<details>

<summary>Where is Anytype installed?</summary>

* In Windows 10 or above, it is usually located:\
  `C:\Users\<username>\Appdata\Local\Programs\anytype`\
  **username** stands for the name of your user aka working directory.
* For MacOS, it's: `HDD > Users >`_`Username`_`> Library > Application Support > anytype`
* For Linux, you'll find your work directory in `~/.config/anytype`
* For Android, it’s your default location, usually: \_device/data/app\_​.\
  We also store some caches: _device/data/data/io.anytype.app_\
  Anytype directory is stored in a protected app data folder, which isn’t accessible by the user on Android devices.
* For iOS, it's the standard install path determined by the iOS.

</details>

<details>

<summary>Are there any network requests when using local-only mode?</summary>

We can guarantee that there are no network requests to our Anytype Network, but our telemetry will still send requests (you will be able to opt-out later on). Additionally, the client still needs to to send requests for some of the features (embedding blocks, fetching bookmarks, etc.) to work properly.

</details>

<details>

<summary>What to do if I'm asked to enter my key / recovery phrase each time on Linux?</summary>

Linux users may be asked for their Key each time they log in. To resolve this issue, please install a keychain. The most popular is [GNOME Keyring](https://wiki.gnome.org/action/show/Projects/GnomeKeyring?action=show\&redirect=GnomeKeyring). Additionally, ensure that you have met all the [dependencies](https://github.com/anyproto/anytype-ts#dependencies) beforehand.

</details>

<details>

<summary>Why is there no browser version of Anytype?</summary>

There's no browser version of the app. Anytype is a stand-alone software, that works on desktop or mobile devices. There are many points of vulnerability in-browser apps that would compromise our commitment to data security and encryption.

</details>

<details>

<summary>Can I use two separate Vaults at the same time?</summary>

Here's a tweak that works only on desktop: you need to create a separate shortcut for your other Vault and add the `--user-data-dir="$path"` flag to the launch command (i.e. `--user-data-dir="D:\Anytype"`).

</details>

<details>

<summary>Can I install Anytype on a Chromebook?</summary>

There are a few ways you can install Anytype on a Chromebook, but probably the easiest one is to use an [AppImage](https://download.anytype.io). For the full guide from one of our community members, please click [here](https://community.anytype.io/t/guide-to-use-anytype-on-a-chromebook/12181).

</details>

<details>

<summary>Does Anytype have a bug bounty program?</summary>

As a non-profit organization that hasn’t reached a sustainable income yet, we don’t have any guaranteed bug bounty program. If you can prove that you found a critical vulnerability in our applications but don’t want to disclose it, we can discuss a potential reward. Please check this [page](https://github.com/anyproto/.github/blob/main/docs/SECURITY.md) from our GitHub for more information.

</details>

<details>

<summary>What can I do if I can't open Anytype links through a browser?</summary>

You can still open any Anytype links by simply pasting them in the global search menu within Anytype and hitting enter.

</details>

<details>

<summary>How can I create columns?</summary>

You can use the orange 'handle' to the left of each block to create parent/child blocks or new columns in your editor by dragging and dropping them.

<div><figure><img src="../../../.gitbook/assets/image (70).png" alt=""><figcaption></figcaption></figure> <figure><img src="../../../.gitbook/assets/image (71).png" alt=""><figcaption></figcaption></figure></div>

</details>

<details>

<summary>Why can't I search inside objects on iOS?</summary>

Currently, this feature is unavailable on iOS.

</details>

<details>

<summary>Why can't I search or batch select objects inside queries on mobile?</summary>

These features are currently unavailable on both iOS and Android.

</details>

<details>

<summary>Why does it say that my key is too short?</summary>

This issue is usually resolved by adding a space at the end after pasting your key.

</details>
