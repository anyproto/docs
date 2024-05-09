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

<summary>How can I recover data after a suspected database corruption (Win 11)?</summary>

If you’re experiencing issues with Anytype, such as after a sudden power loss, and suspect database corruption, follow these step-by-step instructions to recover your data:

**Step 1**: Locate the Anytype Account Data

1. Open File Explorer: Press `Win + E` to open File Explorer.
2. Access the AppData Folder: In the address bar, type `%AppData%` and press `Enter`. This takes you to the `Roaming` folder inside `AppData`.
3. Navigate to Anytype Data Folder: Go to the Anytype folder by following this path:
4. `Anytype > data > <accountId>` or `Anytype > beta > data > <accountId>` in case you are on the Pre-release(beta) channel in anytype
5. Replace `<accountId>` with your specific account ID.

**Step 2:** Rename the Localstore Database

1. Find the Localstore Folder: Inside the Anytype data folder, look for a folder named `localstore`.
2. Rename the Localstore Folder: Right-click on the `localstore` folder and select `Rename`. Change the name to something like `localstore_backup`. This step ensures that Anytype will create a new localstore database when it runs next, while keeping your old data safe in the renamed folder.

**Step 3:** Restart Anytype

1. Launch Anytype: Open the Anytype application on your computer.
2. Check for Normal Operation: Anytype should now launch without issues. It will create a new localstore database automatically.

If after these steps Anytype still doesn’t launch, probably you have spacestore database corrupted. Please take a look at this instruction [A tool to fix the 'Anytype Helper Crashed' Issue 2](https://community.anytype.io/t/a-tool-to-fix-the-anytype-helper-crashed-issue/13653).

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

<summary>Can I use two separate vaults at the same time?</summary>

There's a hack that can be done on desktop only. You will need to create a separate shortcut for your other vault, and add the `--user-data-dir="$path"` flag to the launch command (i.e. `--user-data-dir="D:\Anytype"`).

</details>

<details>

<summary>Where can I find keyboard shortcuts / hotkeys?</summary>

You can check all keyboard shortcuts in the app by clicking on `? > Keyboard shortcuts` in the bottom right corner of the app.

</details>
