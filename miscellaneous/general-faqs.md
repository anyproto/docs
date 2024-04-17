# General FAQs

<details>

<summary>Are there any network requests when using local-only mode?</summary>

We can guarantee that there are no network requests to our Anytype Network, but our telemetry will still send requests (you will be able to opt-out later on). Additionally, the client still needs to to send requests for some of the features (embedding blocks, fetching bookmarks, etc.) to work properly.

</details>

<details>

<summary>Login issues on Linux</summary>

Linux users may be asked for their Recovery Phrase each time they log in. To resolve this issue, please install a keychain. The most popular is [GNOME Keyring](https://wiki.gnome.org/action/show/Projects/GnomeKeyring?action=show\&redirect=GnomeKeyring). Additionally, ensure that you have met all the [dependencies](https://github.com/anyproto/anytype-ts#dependencies) beforehand.

</details>
