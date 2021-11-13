# Privacy & Security

## Privacy

All your data is private in Anytype alpha. Only you have the encryption keys. No one at Anytype is able to decrypt your data. So if you lose your phrase, we can’t restore the access. No one in Anytype or anyone else can read the content of your Anytype.

### Keychain

Your keychain phrase is the login and passphrase at the same time.

Similar to Bitcoin — this mnemonic is the represenation of your master key generated on the sign up. It is not possible to change it or automatically migrate all your data to a new key if the current one is compromised or forgotten.

For now we can’t do anything about it rather than creating a new account and importing all the data from the markdown backup. The invitation key can be used only once. Your keychain become stored in OS wallet application after sign up, so app can login automatically when start up.

{% hint style="info" %}
We are thinking about logic to provide possibilities like recovery, migration, and keychain changing with the second factor in the future.
{% endhint %}

### Local Anytype data folder itself is not encrypted

Anytype stores data in non-encrypted way locally. We have a prerequisite that user’s machine is non-compromised and trusted. Basically, if a machine is compromised there are plenty of attacking vectors including RAM scanning and passphrase keylogging, so it is useless. We will definitely make additional encryption later. **For now we recommend turning HDD encryption and device passlock on.**

### Tech details

There is some technical details on encryption and data storage:

* Anytype stores changes for each object you’ve created
* Every object’s change has 2 encryption layers with different keys
* First layer is used to connect changes within an object (e.g. all this encrypted data belongs to the object with id \<abc>)
* Second layer is used to encrypt the actual data
* When you create a new change for an object we periodically send it to our backup node(with only the first-layer key). More info about sync [here](syncing-and-p2p.md).
* Anytype backup nodes have access to the first layer key, so it can group changes for the object and send them in one pack when you want to restore your data
* Anytype backup nodes HAVE NO access to the second layer key, so it can’t read the actual changes data
