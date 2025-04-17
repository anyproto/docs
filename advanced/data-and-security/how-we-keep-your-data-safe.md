# Privacy & Encryption

### Privacy <a href="#privacy" id="privacy"></a>

All of your data is private in Anytype. Only you have the encryption keys. No one at Anytype can decrypt your data. So if you lose your phrase, we can’t restore access. Likewise, no one in Anytype or anyone else can read the content of your Anytype.

### Encryption <a href="#keychain" id="keychain"></a>

* Your objects are stored both locally and on nodes in an encrypted format, which can only be decoded using encryption keys. They are different for each document, and we have a certain hierarchy of keys.
* To be able to search through the documents efficiently, we create indexes of your data locally on the basis of the encrypted objects. Think of that as two different storages: one for data, the other for indexes. We decrypt these encrypted objects on the fly with your keys, perform some logic and then save the results (i.e. indexes) locally. These indexes are not encrypted, but here we assume that only you have access to your local data, i.e. the access to your local computer is not compromised.
* These indexes are not synced anywhere and they stay only on your computer. For example, if you have two devices, each of them will have its own index storage

{% hint style="danger" %}
We have a prerequisite that the user’s machine is non-compromised and trusted. Basically, if a device is compromised, there are plenty of attack vectors, including RAM scanning and passphrase keylogging, which makes local encryption much less useful. We will definitely make additional encryption later. **For now, we recommend turning HDD encryption and device password on.**
{% endhint %}

#### Tech details <a href="#tech-details" id="tech-details"></a>

Here are some technical details on encryption and data storage:

* Anytype stores the history of changes for each object you’ve created.
* Every object’s change has 2 encryption layers with different keys.
* The first layer is used to connect changes within an object, e.g. "all this encrypted data belongs to the object with id \<abc>".
* The second layer is used to encrypt the actual data. We use AES with stream encryption with CFB mode.
* When you create a new change for an object, we periodically send it to our backup node (with only the first-layer key). More info about sync [here](https://tech.anytype.io/any-sync/overview).
* Anytype backup nodes have access to the first layer key, so it can group changes for the object and send them in one pack when you want to restore your data.
* Anytype backup nodes HAVE NO access to the second layer [Broken link](broken-reference "mention"), so it can’t read the actual changes to the data.

### Key

#### Why do we use a seed phrase as a Key?

The primary purpose of a seed phrase is to provide a secure and convenient method for backing up and restoring encrypted information. By utilizing a seed phrase, we can recover our private keys and access our data even if our devices are lost, stolen, or damaged. It acts as a master key that unlocks the gateway to our data, making it an indispensable tool for long-term data preservation and security.

Seed phrases follow a standardized protocol called BIP-39 (Bitcoin Improvement Proposal 39), which ensures compatibility across different wallets and applications. The BIP-39 protocol also introduces a checksum to detect transcription errors, minimizing the risk of loss due to human error.

#### Can Anyone Obtain My Key?

The strength of your key lies in its ability to safeguard your digital assets. When properly generated, managed, and stored, it is nearly impossible for anyone to obtain your key without your consent or knowledge. Keys are generated using complex mathematical algorithms, and the sheer number of possible combinations makes it extremely challenging for an attacker to guess or brute-force their way to your key.

{% hint style="info" %}
**Combinations:** 5,444,517,870,735,015,415,413,993,718,908,291,383,296

**Cost To Crack:** $38,029,518,006,846,883,000,000,000 USD
{% endhint %}

However, it's crucial to understand that the responsibility of protecting your key ultimately lies with you. While it may be tempting to store it digitally for convenience, these methods can introduce vulnerabilities. Instead, it is recommended to write down your key on a physical medium, and store it securely in a location known only to you. Avoid storing your Key on devices connected to the internet or in cloud storage, as they can be compromised by hackers or unauthorized access.

#### What's the risk of creating two Vaults with the same Key?

The chance of two people having the same 128-bit mnemonic is about 1 in 2¹²⁸ (roughly 3.4 × 10³⁸)—vastly more than the number of grains of sand on Earth. Even generating billions of keys per second for 100 years wouldn’t come close to causing a collision. In short, key collisions are virtually impossible.
