# Storage & Deletion

### Storage <a href="#storage" id="storage"></a>

Anytype is offline first; hence, all data you create will be stored locally first. After that, the data is synced to the backup node and your devices for redundancy. We use a private [IPFS](https://docs.ipfs.tech/concepts/what-is-ipfs/) network to handle storage. It is a Peer-To-Peer file system that facilitates decentralized data storage across devices. Local P2P is supported, meaning that you can sync between your devices directly if they are connected through the same local network. This will work no matter what network mode you use, and it's the only way to sync between your devices if you are using local-only mode.

{% hint style="info" %}
It will be possible to change your storage location in the [future](https://github.com/orgs/anyproto/projects/1/views/1?pane=issue\&itemId=29227794). You might consider using a [workaround from our user](https://community.anytype.io/t/custom-storage-location/994) as a temporary solution for Windows and MacOS.
{% endhint %}

#### Media <a href="#media" id="media"></a>

Media files are not directly downloaded in overall syncing to save bandwidth. Instead, when that file is requested, it is streamed to your device from the backup node or your devices on the network. For example, if you have a 4K Video, it will be streamed from the backup node or P2P devices to your device. So when you open an object with an image, it downloads. When you press play on video & audio, it begins to download. After that, this file will be stored in the application cache.

Furthermore, we use the deduplication feature to reduce storage. For example, if the same picture is uploaded three times, there is only one image copy stored to reduce storage consumption.

You can remove all the media content from your device via the clear cache option in iOS and Android. This will remove all the data altogether and force the app to sync once again entirely. Since the media download works on-premise, you will remove all cached media and clear some storage.

{% hint style="info" %}
Because of a legacy file system, some files might disappear from your graph if they are no longer linked to any objects. But fear not; all of your files are still there. We are working on [fixing the problem](https://community.anytype.io/t/are-unlinked-images-automatically-deleted/10810/3?u=isle9) already.
{% endhint %}

### Deletion <a href="#deletion" id="deletion"></a>

<figure><img src="https://files.gitbook.com/v0/b/gitbook-x-prod.appspot.com/o/spaces%2FJbcKxgThRdSa4vZyLbvH%2Fuploads%2Fgit-blob-dcb526128401892f1a4773091dbf735febb4a875%2FScreenshot%202021-11-02%20at%2016.25.23.png?alt=media" alt=""><figcaption><p>Complete deletion in Bin</p></figcaption></figure>

At the moment you can only delete the Objects that you've created inside Anytype. At first, you can move them to the bin. Secondly, you can remove them completely from all devices. All your devices will also delete them when getting online. This action is irreversible, so please be careful.

The deleted objects are still accessible in read-only mode, either from the bin, or through previously added links. You are also able to restore these objects directly through the read-only mode without needing to go through the bin.

Types and relations created by Anytype can't be deleted at the moment, but might be deletable in future releases.
