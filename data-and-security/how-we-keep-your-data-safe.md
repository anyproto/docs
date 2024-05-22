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
* Anytype backup nodes HAVE NO access to the second layer [what-is-a-recovery-phrase.md](what-is-a-recovery-phrase.md "mention"), so it can’t read the actual changes to the data.
