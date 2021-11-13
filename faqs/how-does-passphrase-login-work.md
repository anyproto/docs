# How does passphrase login work?

To keep your Data secure we, use the BIP39 Algorithm to derive keychain phrases and use the process of [**Key Derivation Function**](https://en.wikipedia.org/wiki/Key\_derivation\_function) to get all the information that needs to be associated with your passphrase.

### Steps

1. Your keychain phrase is used to derive your account's [**private key**](https://en.wikipedia.org/wiki/Public-key\_cryptography) using the [**BIP39 Algorithm**](https://medium.com/coinmonks/mnemonic-generation-bip39-simply-explained-e9ac18db9477)**.**
2. Then your private key is further used to derive your profile page with a [**Textile-DB thread ID**](https://github.com/textileio/go-threads)** **and the encryption key. This is how we ensure that your account is associated with your ID.
3. Then your private key is used to derive the ID and encryption key for the [**ThreadsDB**](https://github.com/textileio/go-threads#running-threaddb) that contains encryption keys for the rest of the [object](../fundamentals/object/ "mention") you have in Anytype.
