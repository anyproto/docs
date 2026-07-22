# Sync & Backup

Anytype is built on local-first principles. It combines the seamless experience of modern cloud applications with the privacy, security, and ownership of local software. Traditional cloud apps store your data on centralized servers that they can access at anytime—all that protects you in reality is a privacy policy.&#x20;

Everything in Anytype lives on your devices locally, is encrypted with keys that only you control, while our protocol handles syncing and backup seamlessly in the background. You always retain full ownership of your data and can never be locked out.&#x20;

## Why it matters

Local-first sync means that you can retain your ownership and control over all your data while gaining the benefits of using the internet to sync between your devices and collaborate with others. No compromises.&#x20;

## How It Works

Anytype’s architecture consists of three core components: Local Storage, Network Sync, and Backups.

#### Local Storage & Encryption

1. On-Device Storage: Everything is stored locally, making your data always accessible and fast.&#x20;
2. Encryption: All content is encrypted locally using your Key before it ever leaves your device to sync.&#x20;

#### Sync & Network Modes

By default, everyone joins the **Anytype Network** when they create a new vault. The provides local-first sync, where:&#x20;

Anytype offers three ways to handle multi-device synchronization and network connectivity:

1\. Standard Local-First Mode _(Default)_

* Peer-to-Peer (P2P): When two of your devices are online, they sync changes directly with each other over encrypted channels.
* Encrypted Backup Node: If your other devices are offline, Anytype’s backup node receives and stores _end-to-end encrypted blobs_ of your changes. When your secondary device comes back online, it fetches those encrypted blobs and decrypts them locally.

2\. Self-Hosted Mode

* Custom Control: You can host your own Anytype Backup Node on a private server or home lab.
* Private Routing: Your devices sync through your self-hosted node instead of Anytype's infrastructure, giving you complete cloud-like syncing on your own hardware.

3\. Local-Only Mode _(Experimental)_

* Zero Server Interaction: Disables communication with all backup nodes entirely.
* Local Network Sync Only: Multi-device syncing works strictly over your local network (Wi-Fi/LAN) when devices are active at the same time.
* Network Isolation: Ideal for air-gapped devices or ultra-strict threat models.

#### Backups & Recovery

How data recovery works depends on your active mode:

Standard Local-First & Self-Hosted Modes

* Automated Recovery: Because encrypted copies of your data exist on the backup node, losing a device is not catastrophic.
* Seamless Restore: Logging into a new device with your Recovery Passphrase pulls your encrypted vault down from the backup node and decrypts it locally.

















By default, everyone joins the **Anytype Network** when they create a new vault. They can later switch to either [self-hosted.md](self-hosted.md "mention") or [local-only.md](local-only.md "mention") if they wish.

Every Anytype user has access to a remote backup node provided by Anytype with a free storage capacity that can be increased with membership. Objects and other content have no impact on this limit; only files are limited. If you go over the limit, a warning will appear, and you'll be able to ask for more storage.

Our infrastructure is hosted in Zurich based data centers within Europe. Production currently runs on Google Cloud Platform, with plans to move to dedicated European hosted servers.

The domains we use for our Anytype network are:

* For syncing: `*.anyclub.org`
* For our analytics: `*.anytype.io`

### How to switch back to Anytype network

We strongly recommend using dedicated identities for each network. If you are switching from a Self-hosted network, export all your channels, and import them into a new identity after switching the network mode.

Please note that all your devices should be manually switched to Anytype Network mode.

#### Desktop

1. Log out from your current identity.
2. On the onboarding screen, click a gear icon in the top right corner.
3. In the “Network” field choose the “Anytype” option.
4. Click the “Save” button.
5. Create a new identity or log in with an existing one.

<figure><img src="../../../.gitbook/assets/image (43).png" alt=""><figcaption></figcaption></figure>

#### Mobile

1. Log out from your current identity.
2. On the onboarding screen, click a gear icon in the top right corner.
3. Click on “Anytype” in the “Networks” sub-menu.
4. Create a new identity or log in an existing one.

<figure><img src="../../../.gitbook/assets/Screenshot_20240411-104810_Anytype2.png" alt="" width="375"><figcaption></figcaption></figure>
