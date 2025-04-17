# Networks & Backup

By default, everyone joins the **Anytype Network** when they create a new vault. They can later switch to either [local-only.md](local-only.md "mention") or [self-hosted.md](self-hosted.md "mention") if they wish.

Every Anytype user has access to a remote backup node provided by Anytype. Its capacity is currently limited to 1 GB. Objects and other content have no impact on this limit; only files are limited. If you go over the limit, a warning will appear, and you'll be able to ask for more storage.

Our backup nodes are located in Switzerland, and we use AWS (Amazon Web Services).

The domains we use for our Anytype network are:

* For syncing: `*.anyclub.org`
* For our analytics: `*.anytype.io`

### How to switch back to Anytype network

We strongly recommend using dedicated identities for each network. If you are switching from a Self-hosted network, export all your spaces, and import them into a new identity after switching the network mode.

Please note that all your devices should be manually switched to Anytype Network mode.

#### Desktop

1. Log out from your current identity.
2. On the onboarding screen, click a gear icon in the top right corner.
3. In the “Network” field choose the “Anytype” option.
4. Click the “Save” button.
5. Create a new identity or log in with an existing one.

<figure><img src="../../../.gitbook/assets/image (51) (1).png" alt=""><figcaption></figcaption></figure>

#### Mobile

1. Log out from your current identity.
2. On the onboarding screen, click a gear icon in the top right corner.
3. Click on “Anytype” in the “Networks” sub-menu.&#x20;
4. Create a new identity or log in an existing one.

<figure><img src="../../../.gitbook/assets/Screenshot_20240411-104810_Anytype2.png" alt="" width="375"><figcaption></figcaption></figure>
