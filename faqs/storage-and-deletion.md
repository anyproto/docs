# Storage & Deletion

## Storage

Anytype is Offline first; hence, all data you create will be stored locally first. After that, the data is synced to the backup node and your devices for redundancy.

We use a private IPFS network and [ThreadDB](https://docs.textile.io/threads/) to handle storage. It is a Peer-To-Peer file system that facilitates decentralized data storage across devices. Furthermore, we use the deduplication feature to reduce storage. For example, if the same picture is uploaded three times, there is only one image copy stored to reduce storage consumption.

{% hint style="info" %}
You can read more about IPFS here: [we-are-using-ipfs.-what-is-that.md](../faqs/we-are-using-ipfs.-what-is-that.md "mention").
{% endhint %}

### Media

Media files are not directly downloaded in overall syncing to save bandwidth. Instead, when that file is requested, it is streamed to your device from the backup node or your devices on the network. For example, if you have a 4K Video, it will be streamed from the backup node or P2P devices to your device.

So when you open an object with an image, it downloads. When you press play on video & audio, it begins to download. After that, this file will be stored in the application cache.

## Deletion

![Complete deletion in Bin](<../.gitbook/assets/Screenshot 2021-11-02 at 16.25.23.png>)

At the moment you can delete only the [fundamental-concepts.md](../fundamental-concepts.md "mention") that you create inside Anytype. At first, you can move them to a bin that will remove them from navigation. Secondly, you can remove them completely from all devices. All your devices will also delete them when getting online.

{% hint style="warning" %}
This action is irreversible, so please be careful.
{% endhint %}

### Media

{% hint style="warning" %}
Objects like Media and those with Anytype (Types, Relations) might be deleted in further releases.
{% endhint %}

You can delete all the content via the clear cache option in iOS and Android. This will remove all the data altogether and force the app to sync once again entirely. Since the media download works on-premise (take a look on[#media-1](storage-and-deletion.md#media-1 "mention")), you will remove all cached media and clear some storage.

## Root Folder

The Anytype Root Folder is a variable based on the OS where all your local data is stored. Currently, it is not possible to change the location of this folder. However, this functionality will be added at a later date.

## Filesystem integration

Anytype does not have a way to reference files from the OS files system. So all the files are getting copied when you drop media and files inside Anytype. We will introduce this feature later.

{% hint style="success" %}
By the way, you can check our roadmap in the [Community Forum](https://community.anytype.io/t/release-plan-a-general-roadmap/1283).
{% endhint %}
