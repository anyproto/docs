# FAQs

## General

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
  * macOS Catalina 10.15+
  * 64-bit Ubuntu 18.04+, Debian 10+, openSUSE 15.5+, or Fedora Linux 38+
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

<summary>What happened to the old homepage?</summary>

<img src="../../../.gitbook/assets/w=3840,quality=80 (1).webp" alt="" data-size="original">

The homepage from the alpha app has been removed, and replaced with the new sidebar and widgets. If you really liked this layout, you can try recreating it using a set with a gallery view or you can try this [gallery experience](https://gallery.any.coop/Made%20by%20Any?experience=legacy_homepage).

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

<summary>What can I do if I get a GLIBCXX error? </summary>

If you are having issues with GLIBCXX, you can install the [latest version](https://download.anytype.io/) , try going through [this](https://community.anytype.io/t/update-45-1-unable-to-launch/26723/4?u=filip) thread to solve the issue or try the (unofficial) [flatpak](https://flathub.org/apps/io.anytype.anytype) version.

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

<summary>Why do I have an Entry Space?</summary>

Vaults created before version 0.44.0 have an Entry Space. You are free to delete this space if no longer needed, or you can migrate your data to a different space by using the [import-export](../../data-and-security/import-export/ "mention") feature.

</details>

## Collaboration

<details>

<summary>How do I create a shared space?</summary>

![](<../../../.gitbook/assets/Space Settings_Shared Space Creation.png>)

Each newly Space you create is _Private_ by default. In the Space settings menu, you’ll see the option to ‘Share’. This will create a share link that you can send to anyone you would like to join your space. At this point, the Space becomes a _Shared_ Space.&#x20;

</details>

<details>

<summary>What access control settings are available in my shared spaces? </summary>

When you create a shared space you are the Space Owner. The Space Owner can change any object in the space, the space name and settings, and is the only one with rights to add and remove members.

Members of the Space have either Viewer or Editor rights. Viewers have read-only access to the Space, while Editors can edit any object in the Space or the Space Name.&#x20;

</details>

<details>

<summary>How do I invite people to my space?</summary>

![](<../../../.gitbook/assets/Anytype Space Sharing_Invite Link.png>)

As a Space owner, once you click 'Share Space' in your space settings, you can generate a shareable invite link. Anyone who you send this link to, can request access to your space.&#x20;

When a new user requests access to your space, you can approve or deny the request and set their access to 'Editor' or 'Viewer'.

</details>

<details>

<summary>How does the invite link work?</summary>

When clicking your invite link, guests who have already installed Anytype will see a popup confirmation screen asking if they would like to join your space. Upon clicking ‘Request to Join’, you will receive a notification for a join request from \[Guest Profile name] to your shared space.

If your guest has never installed Anytype, the invite link will open a unique download page with instructions for installing the application. After having done so, they would need to click the invite link again, which will open the ‘Request to Join’ confirmation popup.

</details>

<details>

<summary>How many people can I invite to my space?</summary>

Explorers can invite up to two additional Editors per shared space. Builders and Co-creators can invite up to nine additional Editors per shared space, and an unlimited number of Viewers.

</details>

<details>

<summary>Can guests of my space use Anytype from local-only mode?</summary>

Unless they are all part of the same local network, guests will need to be connected to the Anytype network in order to see all changes in the space.

</details>

### Memberships&#x20;

<details>

<summary>What happens to my shared spaces if I choose not to renew my membership?</summary>

You can choose _not_ to renew your paid membership up to any moment before the membership cycle renews. Please do so by visiting the site of the payment provider you used to pay for your membership (Stripe, App store, Google Play).

**Your global name**

Your name will be released and free for purchase one year or 3 years from when you first purchased your membership, depending on which kind of membership you purchased

**Your spaces**

When you do not renew your membership, all participants of your shared spaces (including yourself) will see a popup notification with two options: _Delete_ or _Export_ the space. Only if participants export the space and re-import it to a new space, will they continue to have access to the space data through Anytype (though changes will no longer be synced).

**Your data**

Encrypted backups of your data will be deleted from the Anytype backup node after 30 days.

</details>

<details>

<summary>What payment methods can I use?</summary>

All major credit cards are accepted. Memberships are priced in USD and will be converted to your local currency using conversion rates on Stripe, if you purchase your membership from the Desktop app.

If you purchase your membership from the iOS or Android apps, payment will be processed by the App Store or Play Store, and prices will be automatically adjusted to your local currency by the respective platform.

</details>

<details>

<summary>What if I want to add additional members to my space?</summary>

In our next iteration of memberships, we will have a tier for B2B and educational use cases, with the option to add up to 20 additional editors per space.

</details>

<details>

<summary>What happens if I exceed the storage &#x26; sync limits?</summary>

Your spaces will stop syncing with each other through the backup node and use local sync/storage only.&#x20;

</details>

<details>

<summary>How can I request a refund?</summary>

Refunds must be requested within 5 days of payment by e-mailing [support@anytype.io](mailto:support@anytype.io). We can refund only 25% of the membership fee, as we do not receive a refund for having registered your name on the network.&#x20;

</details>

<details>

<summary>Is there a student / educational plan?</summary>

We offer a 50% discount to anyone who contacts us at [membership-upgrade@anytype.io](mailto:membership-upgrade@anytype.io) using their university-associated email address.

</details>
