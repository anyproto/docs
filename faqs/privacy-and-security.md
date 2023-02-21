# Privacy & Security

## Privacy

All of your data is private in Anytype alpha. Only you have the encryption keys. No one at Anytype can decrypt your data. So if you lose your phrase, we can’t restore access. Likewise, no one in Anytype or anyone else can read the content of your Anytype.

### Keychain

Your keychain phrase is the login and passphrase at the same time.

This mnemonic represents your master key generated on the signup, similar to Bitcoin. Changing it is impossible or automatically migrating all your data to a new key if the current one is compromised or forgotten.

We can’t do anything about it but create a new account and import all the data from the markdown backup. The invitation key can be used only once. After signing up, your keychain becomes stored in the OS wallet application, so the app can log in automatically when startup.

{% hint style="info" %}
We are thinking about logic to provide possibilities like recovery, migration, and keychain changing with the second factor in the future.
{% endhint %}

### Local Anytype data folder itself is not encrypted

Anytype stores data in a non-encrypted way locally. We have a prerequisite that the user’s machine is non-compromised and trusted. Basically, if a device is compromised, there are plenty of attack vectors, including RAM scanning and passphrase keylogging, which is useless. We will definitely make additional encryption later. **For now, we recommend turning HDD encryption and device password on.**

### Tech details

Here are some technical details on encryption and data storage:

* Anytype stores changes for each object you’ve created
* Every object’s change has 2 encryption layers with different keys.
* The First layer is used to connect changes within an object (for example, all this encrypted data belongs to the object with id \<abc>)
* Second layer is used to encrypt the actual data. We using AES with stream **encryption** with CFB mode
* When you create a new change for an object, we periodically send it to our backup node(with only the first-layer key). More info about sync [here](syncing-and-p2p.md).
* Anytype backup nodes have access to the first layer key, so it can group changes for the object and send them in one pack when you want to restore your data
* Anytype backup nodes HAVE NO access to the second layer key, so it can’t read the actual changes to the data
