# Data Storage & Deletion

## Storage & Deletion

### Storage <a href="#storage" id="storage"></a>

Anytype is offline first; hence, all data you create will be stored locally first. After that, the data is synced to the backup node and your devices for redundancy. We use a private [IPFS](https://docs.ipfs.tech/concepts/what-is-ipfs/) network and [ThreadDB](https://docs.textile.io/threads/) to handle storage. It is a Peer-To-Peer file system that facilitates decentralized data storage across devices. Furthermore, we use the deduplication feature to reduce storage. For example, if the same picture is uploaded three times, there is only one image copy stored to reduce storage consumption.

#### Media <a href="#media" id="media"></a>

Media files are not directly downloaded in overall syncing to save bandwidth. Instead, when that file is requested, it is streamed to your device from the backup node or your devices on the network. For example, if you have a 4K Video, it will be streamed from the backup node or P2P devices to your device. So when you open an object with an image, it downloads. When you press play on video & audio, it begins to download. After that, this file will be stored in the application cache.

### Deletion <a href="#deletion" id="deletion"></a>

<figure><img src="https://files.gitbook.com/v0/b/gitbook-x-prod.appspot.com/o/spaces%2FJbcKxgThRdSa4vZyLbvH%2Fuploads%2Fgit-blob-dcb526128401892f1a4773091dbf735febb4a875%2FScreenshot%202021-11-02%20at%2016.25.23.png?alt=media" alt=""><figcaption><p>Complete deletion in Bin</p></figcaption></figure>

At the moment you can delete only the [Fundamentals](https://app.gitbook.com/o/Ssa9i5QAuI6HhV4jXCLv/s/JbcKxgThRdSa4vZyLbvH/fundamental-concepts) that you create inside Anytype. At first, you can move them to a bin that will remove them from navigation. Secondly, you can remove them completely from all devices. All your devices will also delete them when getting online. This action is irreversible, so please be careful.

#### Media <a href="#media-1" id="media-1"></a>

Objects like Media and those with Anytype (Types, Relations) might be deleted in further releases. You can delete all the content via the clear cache option in iOS and Android. This will remove all the data altogether and force the app to sync once again entirely. Since the media download works on-premise, you will remove all cached media and clear some storage.

### Root Folder <a href="#root-folder" id="root-folder"></a>
