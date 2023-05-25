# How we keep your data safe



### Privacy <a href="#privacy" id="privacy"></a>

All of your data is private in Anytype. Only you have the encryption keys. No one at Anytype can decrypt your data. So if you lose your phrase, we can’t restore access. Likewise, no one in Anytype or anyone else can read the content of your Anytype.



#### The local Anytype data folder itself is not encrypted <a href="#local-anytype-data-folder-itself-is-not-encrypted" id="local-anytype-data-folder-itself-is-not-encrypted"></a>

Anytype stores data in a non-encrypted way locally. We have a prerequisite that the user’s machine is non-compromised and trusted. Basically, if a device is compromised, there are plenty of attack vectors, including RAM scanning and passphrase keylogging, which is useless. We will definitely make additional encryption later. **For now, we recommend turning HDD encryption and device password on.**

#### Tech details <a href="#tech-details" id="tech-details"></a>

Here are some technical details on encryption and data storage:

* Anytype stores changes for each object you’ve created
* Every object’s change has 2 encryption layers with different keys.
* The First layer is used to connect changes within an object (for example, all this encrypted data belongs to the object with id \<abc>)
* Second layer is used to encrypt the actual data. We using AES with stream **encryption** with CFB mode
* When you create a new change for an object, we periodically send it to our backup node(with only the first-layer key). More info about sync [here](https://app.gitbook.com/o/Ssa9i5QAuI6HhV4jXCLv/s/JbcKxgThRdSa4vZyLbvH/faqs/syncing-and-p2p).
* Anytype backup nodes have access to the first layer key, so it can group changes for the object and send them in one pack when you want to restore your data
* Anytype backup nodes HAVE NO access to the second layer key, so it can’t read the actual changes to the data
