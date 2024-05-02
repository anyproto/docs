---
description: There are no passwords in Anytype - only your key
---

# Key

<figure><img src="../.gitbook/assets/Screenshot 2023-08-17 at 18.31.38.png" alt=""><figcaption><p>You can access your key at any time by navigating to Profile > Settings > Key</p></figcaption></figure>

When you create your vault, you will receive your very own 12 word mnemonic phrase_._ This phrase is generated on-device and is the only way to access your vault and decrypt your data.

Your Key functions as your login and passphrase at the same time. This mnemonic represents your master key generated upon signup, similar to a Bitcoin wallet.

Changing it is impossible, and it's extremely important you keep it safe. You can access it at any time by navigating to Profile > Settings > Key.

### Don't forget to save it!

We do not save a copy of your key, which means that if it's lost, we are not able to assist with recovering your vault. For this reason, we recommend making a digital backup or writing it down and keeping it somewhere safe.

You will need this key each time you login on a new device.

### What is a Key?

Your key, also known as a seed phrase, is a **unique combination of words** that serves as a cryptographic key. A typical Key consists of 12, 18, or 24 words selected from a predefined list of words.

Your key is used to derive your account's [**private key**](https://en.wikipedia.org/wiki/Public-key\_cryptography) using the [**BIP39 Algorithm**](https://medium.com/coinmonks/mnemonic-generation-bip39-simply-explained-e9ac18db9477).

### Why do we use a seed phrase as a Key?

The primary purpose of a seed phrase is to provide a secure and convenient method for backing up and restoring encrypted information. By utilizing a seed phrase, we can recover our private keys and access our data even if our devices are lost, stolen, or damaged. It acts as a master key that unlocks the gateway to our data, making it an indispensable tool for long-term data preservation and security.

Seed phrases follow a standardized protocol called BIP-39 (Bitcoin Improvement Proposal 39), which ensures compatibility across different wallets and applications. The BIP-39 protocol also introduces a checksum to detect transcription errors, minimizing the risk of loss due to human error.

### Can Anyone Obtain My Key?

The strength of your key lies in its ability to safeguard your digital assets. When properly generated, managed, and stored, it is nearly impossible for anyone to obtain your key without your consent or knowledge. Keys are generated using complex mathematical algorithms, and the sheer number of possible combinations makes it extremely challenging for an attacker to guess or brute-force their way to your key.

However, it's crucial to understand that the responsibility of protecting your key ultimately lies with you. While it may be tempting to store it digitally for convenience, these methods can introduce vulnerabilities. Instead, it is recommended to write down your key on a physical medium, and store it securely in a location known only to you. Avoid storing your Key on devices connected to the internet or in cloud storage, as they can be compromised by hackers or unauthorized access.

### Key storage

If you’re using a Mac, Anytype’s default setting is to store your key in the native Keychain Access app. It doesn’t get stored anywhere else. Whether your passwords are backed up to iCloud depends if you have that option enabled in your settings. You can check [Apple’s support page](https://support.apple.com/en-us/HT204085) for more information on iCloud password backups.

We’ve set up this system as a safety net for users who might otherwise lose their Key. We’re pursuing different options for the future, but for the time being, this is how it works.

If you logged in with your key on your mac, then you can find it here:

1. Click and open Finder from the dock.
2. Click on Applications & open Utilities.
3. Open the Keychain Access app.
4. On the sidebar: select Default Keychains: login
5. Find & open your Anytype instance in the list
6. Check the “Show password” box to reveal your key

#### Windows and Linux

On Windows, your key is stored in the [Credentials Manager](https://support.microsoft.com/en-us/windows/accessing-credential-manager-1b5c916a-6a16-889f-8581-fc16e8165ac0).

On Linux, you can use [seahorse](https://wiki.gnome.org/Apps/Seahorse/) to find your key if you are using [GNOME Keyring](https://wiki.gnome.org/action/show/Projects/GnomeKeyring?action=show\&redirect=GnomeKeyring).
