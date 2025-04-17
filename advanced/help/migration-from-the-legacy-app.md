---
description: Instructions for our Alpha testers
---

# Beta Migration

#### **How to migrate?**

If you’ve created content in the Alpha/Legacy version (0.31.\* and older) that you want to keep, you’ll need to migrate it. The process is relatively straightforward:

1.  Update your Desktop Legacy app to the most recent version (0.31.9) via Anytype > Check for updates or [via the link](https://download.anytype.io/?ref=migration\&platform=desktop).

    <div align="left"><figure><img src="../../.gitbook/assets/Check updates.png" alt="" width="331"><figcaption></figcaption></figure></div>
2.  Export from the updated Legacy app: File > Export > Protobuf.

    <div align="left"><figure><img src="../../.gitbook/assets/Anytype Export.gif" alt="" width="336"><figcaption></figcaption></figure></div>
3. [Download](https://download.anytype.io/), install, and open the Beta app.
4. Import your backup to the Beta app.

For more details, please check our [Migration Trail Guide](https://community.anytype.io/t/anytype-legacy-to-beta-migration-trail-guide/9274).

#### **Where to download the latest Alpha (Legacy) app**

If you have already deleted your Alpha app prior to exporting your data from it, you might want to download it again in order to complete the export. You can download the 0.31.9 desktop app for Mac, Windows, and Linux [via the following link](https://download.anytype.io/?ref=migration\&platform=desktop).

#### How can I skip the import backup step?

Instead of migrating, you’ll have the following alternatives:

*   Create a new vault. When the app is launched, pick up Join instead of Login.

    <div align="left"><figure><img src="../../.gitbook/assets/Join Anytype.png" alt="" width="354"><figcaption></figcaption></figure></div>
* Manually import selected Objects one by one from Legacy to Beta. You may want to do this if your Legacy vault / account has become messy but you have a few projects you’d like to carry over to Beta.

For these options, you’ll need to create a new vault, which will generate a new Key.

#### Troubleshooting

* Error "open profile: file does not exist"
  * Reason: this happens with old Legacy versions (e.g. 0.31.0).
  * Solution: update the Legacy app via the instructions above.
* Error "can't run service 'client.clientspace': EOF" \*
