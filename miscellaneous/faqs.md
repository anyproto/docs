# FAQs

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

<summary>Why is RTL not supported?</summary>

RTL is currently only partially supported, but we have plans for full support later on.

</details>

<details>

<summary>What happened to the old homepage?</summary>

<img src="../.gitbook/assets/w=3840,quality=80 (1).webp" alt="" data-size="original">

The homepage from the alpha app has been removed, and replaced with the new sidebar and widgets. If you really liked this layout, you can try recreating it using a set with a gallery view.

</details>

<details>

<summary>Can I use two separate Vaults at the same time?</summary>

Here's a tweak that works only on desktop: you need to create a separate shortcut for your other Vault and add the `--user-data-dir="$path"` flag to the launch command (i.e. `--user-data-dir="D:\Anytype"`).

</details>

<details>

<summary>Where can I find keyboard shortcuts / hotkeys?</summary>

You can check all keyboard shortcuts in the app by clicking on `? > Keyboard shortcuts` in the bottom right corner of the app.

</details>

<details>

<summary>Can I install Anytype on a Chromebook?</summary>

There are a few ways you can install Anytype on a Chromebook, but probably the easiest one is to use an [AppImage](https://download.anytype.io). For the full guide from one of our community members, please click [here](https://community.anytype.io/t/guide-to-use-anytype-on-a-chromebook/12181).

</details>

<details>

<summary>Does Anytype have a bug bounty program?</summary>

As a non-profit organization that hasn’t reached a sustainable income yet, we don’t have any guaranteed bug bounty program. If you can prove that you found a critical vulnerability in our applications but don’t want to disclose it, we can discuss a potential reward. Please check this [page](https://github.com/anyproto/.github/blob/main/docs/SECURITY.md) from our GitHub for more information.

</details>

