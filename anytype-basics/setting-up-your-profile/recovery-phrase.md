---
description: There are no passwords in Anytype - only your recovery phrase.
---

# Recovery Phrase

Your Recovery Phrase functions as your login and passphrase at the same time. This mnemonic represents your master key generated upon signup, similar to a Bitcoin wallet.&#x20;

Changing it is impossible, and it's extremely important you keep it safe.

### Generate your phrase

When you create your account, you will receive your very own _12 word mnemonic phrase._ This phrase is generated on-device and is the only way to access your account and decrypt your data.

<figure><img src="../../.gitbook/assets/image (16).png" alt="" width="375"><figcaption></figcaption></figure>

### Don't forget to save it!

We do not save a copy of your recovery phrase, which means that if it's lost, we are not able to assist with account recovery. For this reason, we recommend making a digital backup or writing it down and keeping it somewhere safe.&#x20;

You will need this phrase each time you login on a new device.

### Login on mobile

You can login on your mobile device (iOS or Android), either by using your recovery phrase or by scanning the QR code on your the 'Recovery Phrase' screen in your desktop app, located by navigating to: Account > Recovery Phrase.&#x20;

Simply launch the Anytype app on your device, tap "Login" and "Scan QR code".&#x20;

<figure><img src="../../.gitbook/assets/image (20).png" alt="" width="375"><figcaption></figcaption></figure>

To access your QR code in the desktop app, navigate to Settings > Recovery Phrase.

<figure><img src="../../.gitbook/assets/Anytype Recovery Phrase.png" alt="" width="375"><figcaption><p>Recovery phrase in Account Settings</p></figcaption></figure>

### Tech

Your recovery phrase is used to derive your account's [**private key**](https://en.wikipedia.org/wiki/Public-key\_cryptography) using the [**BIP39 Algorithm**](https://medium.com/coinmonks/mnemonic-generation-bip39-simply-explained-e9ac18db9477).  Then, your private key is further used to derive your profile page with a [**Textile-DB thread ID**](https://github.com/textileio/go-threads) and the encryption key. This is how we ensure that your account is associated with your ID. Finally, your private key is used to derive the ID and encryption key for the [**ThreadsDB**](https://github.com/textileio/go-threads#running-threaddb) that contains encryption keys for the rest of the content that you have created in Anytype.
