# Local-only

If you prefer to fully keep your data on your device without any server to sync between your desktop and mobile, you can enable Local-Only Mode. This mode disables Anytype's backup node entirely—meaning multi-device syncing will only work over the same local network, and your data lives exclusively on your devices.

{% hint style="danger" %}
**Local-only mode is marked experimental** because manual backup management carries a high risk of accidental data loss. If you choose this mode, ensure you regularly export your data and manage your backups. Anytype has no ability to help you with recovering data loss from local-only mode.&#x20;
{% endhint %}

## How it works

Anytype is built on [local-first principles](https://www.inkandswitch.com/essay/local-first/)—designed for people who love the convenience of modern cloud apps, but refuse to sacrifice their privacy, security, and ownership. To understand how local-only is different from local-first:&#x20;

**Local-Only**

* Storage: Data lives exclusively on your device.
* Syncing: No syncing through a server.&#x20;
* Risk: If your device breaks or gets lost, your data is gone forever.
* Backups: Entirely manual and your personal responsibility.

**Local-First (Anytype Network)**

* Storage: Data lives on your device and works fully offline.
* Syncing: Syncs automatically across your devices via end-to-end encryption whenever you're connected.
* Privacy: Only you hold the decryption keys—Anytype can never read your content.
* Recovery: If you lose all your devices, you can still restore it via Anytype's encrypted backup node.

In summary, local-only means no syncing with servers. Local-first means it works offline, syncs like a cloud app, but is only accessible to you.&#x20;

### Should I use local-only mode?&#x20;

In short: the standard local-first mode using the Anytype Network is almost always the better choice.

Anytype is built private by default. Because your encryption keys are generated locally and never leave your device, your data is completely inaccessible to anyone else—a design verified in our open-source code. The standard Anytype Network mode gives a fantastic balance between security and convenience.&#x20;

By contrast, local-only mode offers very little additional security for the average person while dramatically increasing the risk of unrecoverable data loss. Unless your security model strictly requires complete network isolation (such as running on an air-gapped device), we recommend using standard local-first mode by connecting to the Anytype Network.&#x20;

## How to switch to local-only mode

#### Desktop

1. Log out from your current identity.
2. On the onboarding screen, click a gear icon in the top right corner.
3. In the “Network” field choose the “Local-only” option.
4. Click the “Save” button.
5. Create a new identity or log in with an existing one.

<div data-with-frame="true"><figure><img src="../../.gitbook/assets/image (45).png" alt=""><figcaption></figcaption></figure></div>

#### Mobile

1. Log out from your current identity.
2. On the onboarding screen, click a gear icon in the top right corner.
3. Click on “Local-only” in the “Networks” sub-menu.
4. Create a new identity or log in an existing one.

<div data-with-frame="true"><figure><img src="../../.gitbook/assets/Screenshot_20240411-104810_Anytype2.png" alt="" width="375"><figcaption></figcaption></figure></div>

## Recovering data in local-only mode

In Local-Only Mode, your data is 100% your responsibility. Because Anytype has zero access to your device or encryption keys, we cannot assist with recovering lost, deleted, or corrupted data. There are no remote backups stored on our nodes.&#x20;

**To protect your work from device failure or accidental deletion, you must regularly export and back up your spaces to a secure external location.**

## Third-party services & network drives

Do not place your active Anytype data directory inside a third-party cloud-synced folder (such as Nextcloud, Dropbox, OneDrive, or Google Drive) or on a shared network drive. Doing so introduces severe risks to both your data integrity and your privacy.

1. **High Risk of Database Corruption** — Anytype uses SQLite databases to store your spaces locally. Cloud sync tools constantly monitor and lock files as they detect changes. When a sync tool touches active SQLite files—especially if multiple devices write at the same time—it disrupts database file-locking. This can lead to irreversible database corruption, broken search indexes, and permanent vault failure.
2. **Privacy & Data Leaks** — While your core content is encrypted, Anytype’s working directory also contains unencrypted local indexes required for app performance and search functionality. Syncing this folder to a third-party cloud provider uploads these unencrypted files, exposing private metadata and index data to that provider.

**How to Store Your Data Safely**

* Use Local Storage Only: Ensure your Anytype data directory resides on a standard, non-synced local drive on your device. That is, standard internal storage.&#x20;
* Manual Backups: If you want to use cloud storage for backups, export your spaces manually or back up a static, closed snapshot of your directory while Anytype is not running.

{% hint style="warning" %}
**If you experience data loss in local-only mode, Anytype cannot help with recovery**. You can explore recovery methods based on your setup with at the Anytype community forum or other general forums.&#x20;
{% endhint %}
