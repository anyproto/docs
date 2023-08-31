---
description: There are no passwords in Anytype - only your recovery phrase.
---

# Recovery Phrase

<figure><img src="../.gitbook/assets/Screenshot 2023-08-17 at 18.31.38.png" alt=""><figcaption><p>You can access your recovery phrase at any time by navigating to Profile > Settings > Recovery Phrase.</p></figcaption></figure>

When you create your account, you will receive your very own 12 word mnemonic phrase_._ This phrase is generated on-device and is the only way to access your account and decrypt your data.

Your Recovery Phrase functions as your login and passphrase at the same time. This mnemonic represents your master key generated upon signup, similar to a Bitcoin wallet.

Changing it is impossible, and it's extremely important you keep it safe. You can access it at any time by navigating to Profile > Settings > Recovery Phrase.

### Don't forget to save it!

We do not save a copy of your recovery phrase, which means that if it's lost, we are not able to assist with account recovery. For this reason, we recommend making a digital backup or writing it down and keeping it somewhere safe.

You will need this phrase each time you login on a new device.

### What is a Recovery Phrase?

A Recovery Phrase, also known as a seed phrase, is a **unique combination of words** that serves as a cryptographic key. A typical Recovery Phrase consists of 12, 18, or 24 words selected from a predefined list of words.

Your recovery phrase is used to derive your account's [**private key**](https://en.wikipedia.org/wiki/Public-key\_cryptography) using the [**BIP39 Algorithm**](https://medium.com/coinmonks/mnemonic-generation-bip39-simply-explained-e9ac18db9477).

### Why are We Using a Recovery Phrase?

The primary purpose of a Recovery Phrase is to provide a secure and convenient method for backing up and restoring encrypted information. By utilizing a Recovery Phrase, we can recover our private keys and access our digital assets even if our devices are lost, stolen, or damaged. It acts as a master key that unlocks the gateway to our data, making it an indispensable tool for long-term data preservation and security.

Recovery Phrases follow a standardized protocol called BIP-39 (Bitcoin Improvement Proposal 39), which ensures compatibility across different wallets and applications. The BIP-39 protocol also introduces a checksum to detect transcription errors, minimizing the risk of loss due to human error.

### Can Anyone Obtain My Recovery Phrase?

The strength of a Recovery Phrase lies in its ability to safeguard your digital assets. When properly generated, managed, and stored, it is nearly impossible for anyone to obtain your Recovery Phrase without your consent or knowledge. Recovery Phrases are generated using complex mathematical algorithms, and the sheer number of possible combinations makes it extremely challenging for an attacker to guess or brute-force their way to your Recovery Phrase.

However, it's crucial to understand that the responsibility of protecting your Recovery Phrase ultimately lies with you. While it may be tempting to store it digitally for convenience, these methods can introduce vulnerabilities. Instead, it is recommended to write down your Recovery Phrase on a physical medium, and store it securely in a location known only to you. Avoid storing your Recovery Phrase on devices connected to the internet or in cloud storage, as they can be compromised by hackers or unauthorized access.

### Login issues on Linux

Linux users may be asked for their Recovery Phrase each time they log in. To resolve this issue, please install a keychain. The most popular is [GNOME Keyring](https://wiki.gnome.org/Projects/GnomeKeyring) — check the [discussion on the Community Forum](https://community.anytype.io/t/linux-version-does-not-keep-me-logged-in/4859). Additionally, ensure that you have met all the [dependencies](https://github.com/anyproto/anytype-ts#dependencies) beforehand.
