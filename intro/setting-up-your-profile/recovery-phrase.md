---
description: There are no passwords in Anytype - only your recovery phrase.
---

# Recovery Phrase

{% hint style="danger" %}
Store your Recovery Phrase somewhere safe and share it with no one!
{% endhint %}

<figure><img src="../../.gitbook/assets/Screenshot 2023-08-17 at 18.31.38.png" alt=""><figcaption><p>You can access your recovery phrase at any time by navigating to Profile > Settings > Recovery Phrase.</p></figcaption></figure>

When you create your account, you will receive your very own 12 word mnemonic phrase_._ This phrase is generated on-device and is the only way to access your account and decrypt your data.

Your Recovery Phrase functions as your login and passphrase at the same time. This mnemonic represents your master key generated upon signup, similar to a Bitcoin wallet.

Changing it is impossible, and it's extremely important you keep it safe. You can access it at any time by navigating to Profile > Settings > Recovery Phrase.

### Don't forget to save it!

We do not save a copy of your recovery phrase, which means that if it's lost, we are not able to assist with account recovery. For this reason, we recommend making a digital backup or writing it down and keeping it somewhere safe.

You will need this phrase each time you login on a new device.

### Tech

Your recovery phrase is used to derive your account's [**private key**](https://en.wikipedia.org/wiki/Public-key\_cryptography) using the [**BIP39 Algorithm**](https://medium.com/coinmonks/mnemonic-generation-bip39-simply-explained-e9ac18db9477).
