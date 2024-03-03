# 存储与删除

### 存储 <a href="#storage" id="storage"></a>

Anytype 一开始是离线的；因此，你创建的所有数据将首先存储在本地。之后，数据会同步到备份节点和你的设备，以实现冗余。我们使用私有 [IPFS](https://docs.ipfs.tech/concepts/what-is-ipfs/) 网络来处理存储。这是一个点对点文件系统，有利于跨设备分散存储数据。支持本地 P2P，也就是说，如果设备连接到了相同的本地网络，就可以直接在设备间同步。无论你使用哪种网络模式，本地 P2P 都会正常工作，如果只使用本地模式（local-only），它也是在设备间同步的唯一方法。

{% hint style="info" %}
[未来](https://github.com/orgs/anyproto/projects/1/views/1?pane=issue\&itemId=29227794) 你将可以更改你的存储位置。你可以考虑使用 [来自我们用户的替代方法](https://community.anytype.io/t/custom-storage-location/994) 作为 Windows 和 MacOS 上的临时解决方案。
{% endhint %}

#### 媒体 <a href="#media" id="media"></a>

为节省带宽，整体同步过程中不会直接下载媒体文件。相反，当你请求某个文件时，它会从备份节点或你在网络上的设备流式传输到你的设备。例如，如果你有一个 4K 视频，它将从备份节点或 P2P 设备流式传输到你的设备。因此，当你打开一个包含图像的对象时，它才会下载。当你播放视频和音频时，它才会开始下载。之后，文件将会存储在应用程序缓存中。

此外，我们还使用重复数据删除功能来减少存储空间。例如，如果同一张图片被上传了三次，则只会存储一个图片副本，以减少存储的消耗。

你可以通过 iOS 和 Android 中的“清除缓存”选项来删除设备中的所有媒体内容。这将完全删除所有数据，并强制应用程序再次完整同步一次。由于媒体下载是按需发生的，删除所有已缓存的媒体将清理出一些存储空间。

{% hint style="info" %}
由于采用的是传统文件系统，如果某些文件不再与任何对象链接，它们可能会从你的图谱中消失。不过不用担心，你的所有文件都还在。我们已经在努力 [解决这个问题](https://community.anytype.io/t/are-unlinked-images-automatically-deleted/10810/3?u=isle9)。
{% endhint %}

### 删除 <a href="#deletion" id="deletion"></a>

<figure><img src="https://files.gitbook.com/v0/b/gitbook-x-prod.appspot.com/o/spaces%2FJbcKxgThRdSa4vZyLbvH%2Fuploads%2Fgit-blob-dcb526128401892f1a4773091dbf735febb4a875%2FScreenshot%202021-11-02%20at%2016.25.23.png?alt=media" alt=""><figcaption><p>从废纸篓中完全删除</p></figcaption></figure>

目前，你只能删除在 Anytype 中创建的【对象】。首先，你可以将它们移到废纸篓。其次，你可以将它们从所有设备中完全删除。你的所有设备在联机时都将删除它们。这个操作是不可逆的，因此请务必小心。

被删除的对象仍然可以通过只读模式访问，可以从废纸篓访问，也可以通过之前添加的链接访问。你也可以直接通过只读模式还原这些对象，而不用去废纸篓。

由 Anytype 创建的类型和关联目前无法被删除，但在未来的版本中可能能被删除。
