# Privacy & Encryption

Most modern software runs on corporate cloud servers, where companies can view your data, monetize it, and lock you out at will. In those systems, you're effectively asking permission to access your own digital life.&#x20;

Anytype is fundamentally different: you are the sole, permanent owner of your digital world. Digital sovereignty isn't a feature of Anytype — it's a core design principle.

## Privacy

Anytype's architecture ensures privacy is mathematically enforced in code, not promised in a policy. In practice, this means:

* **You control access.** Only you can access your spaces and grant access to others — not even Anytype can see your content.
* **No permission required.** You don't need anyone's approval to access your data, not even Anytype's.
* **You can leave anytime.** Your data goes with you, and Anytype can't stop you.

#### How it works

* **Local key generation.** Your cryptographic [Key](../../basics/key.md) is generated locally on your device when you create your [Vault](../../basics/vault-and-key.md). It's never transmitted over the internet or stored on Anytype's servers — only you have it.
* **No master recovery.** Because Anytype holds no keys to your account, we can't reset your password or recover your account if you lose access. Losing your key means losing access to your data permanently.
* **Blind data sync.** All your content is encrypted before it syncs across devices, so Anytype only ever acts as a blind messenger — passing encrypted data along without being able to read it.

## Encryption

Anytype encrypts your data using a layered key system, so that even the infrastructure helping sync and back up your data can't read it. In practice, this means:

* **Objects are encrypted at rest.** Your objects are stored — both locally and on syncing nodes — in an encrypted format that can only be decoded with encryption keys. Each document has its own key, organized under a broader key hierarchy.
* **Indexes stay local and unencrypted.** In order to search your documents efficiently, Anytype builds local indexes from your encrypted objects, decrypting them on the fly with your keys. These indexes are stored separately from the encrypted data itself and aren't encrypted — this assumes your local device hasn't been compromised.
* **Indexes never sync.** Your indexes remain only on the device that created them. If you use two devices, each maintains its own independent index storage.

#### How it works

While Anytype has robust encryption, it ultimately assumes the device you're using is safe. If a device is compromised, local encryption offers limited protection against many attacks. We recommend taking your device security very seriously:&#x20;

1. Require a device password.&#x20;
2. Enable disk encryption.&#x20;
3. Lock your device every time it is unattended.&#x20;
4. Don't share access to your device.&#x20;

<details>

<summary>Technical Details</summary>

* Anytype stores the history of changes for each object you’ve created.
* Every object’s change has 2 encryption layers with different keys.
* The first layer is used to connect changes within an object, e.g. "all this encrypted data belongs to the object with id \<abc>".
* The second layer is used to encrypt the actual data. We use AES with stream encryption with CFB mode.
* When you create a new change for an object, we periodically send it to our backup node (with only the first-layer key). More info about sync [here](https://tech.anytype.io/any-sync/overview).
* Anytype backup nodes have access to the first layer key, so it can group changes for the object and send them in one pack when you want to restore your data.
* Anytype backup nodes have no access to the second layer, so it can’t read the actual changes to the data.

</details>

For more details, please [see here](https://tech.anytype.io/any-sync/overview?id=encryption).&#x20;
