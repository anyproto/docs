# Storage & Deletion

### Storage <a href="#storage" id="storage"></a>

Anytype is offline first; hence, all data you create will be stored locally first. After that, the data is synced to the backup node and your devices for redundancy. We use a private [IPFS](https://docs.ipfs.tech/concepts/what-is-ipfs/) network to handle storage. It is a Peer-To-Peer file system that facilitates decentralized data storage across devices. Local P2P is supported, meaning that you can sync between your devices directly if they are connected through the same local network. This will work no matter what network mode you use, and it's the only way to sync between your devices if you are using local-only mode.

#### Media <a href="#media" id="media"></a>

Media files are not directly downloaded in overall syncing to save bandwidth. Instead, when that file is requested, it is streamed to your device from the backup node or your devices on the network. For example, if you have a 4K Video, it will be streamed from the backup node or P2P devices to your device. So when you open an object with an image, it downloads. When you press play on video & audio, it begins to download. After that, this file will be stored in the application cache.

Furthermore, we use the deduplication feature to reduce storage. For example, if the same picture is uploaded three times, there is only one image copy stored to reduce storage consumption.

You can remove all the media content from your mobile device via the clear cache option in iOS and Android. This will remove all the data altogether and force the app to sync once again entirely. Since the media download works on-premise, you will remove all cached media and clear some storage.

You can also manage your files on desktop by going into `Space settings -> Manage Space -> Manage files`.

{% hint style="info" %}
Files are stored inside `flatfs dir` in encrypted fragments, so they can’t be accessed outside of Anytype.
{% endhint %}

### Deletion <a href="#deletion" id="deletion"></a>

To delete objects in Anytype, you will first need to move them to the [finding-your-objects.md](finding-your-objects.md "mention"). Afterwards, you can remove them completely from all devices by permanently deleting them from the bin. All your devices will also delete them when getting online. This action is irreversible, so please be careful.

The deleted objects are still accessible in read-only mode, either from the bin, or through previously added links. You are also able to restore these objects directly through the read-only mode without needing to go through the bin.

Types and Properties created by Anytype can't be deleted at the moment, but might be deletable in future releases.
