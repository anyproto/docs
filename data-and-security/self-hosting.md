# Backup and self-hosting

#### Backup node

Every Anytype user has access to a remote backup node provided by Anytype. Its capacity is currently limited to 1 Gb. These nodes are located in Switzerland.



**How to remove Anytype backup node**\
It's also possible to use p2p sync between your devices, you can [block Anytype network traffic](https://community.anytype.io/t/is-there-a-way-to-limit-storage-of-data-only-local/6982) (Anytype & Anytype Helper) via your firewall.



**How to self-host Anytype**

If you don’t want to use Anytype backup node, you can self-host your own using [this guide](https://tech.anytype.io/how-to/self-hosting). It is our first step in this direction, so it requires some technical skills from users and depends on several external solutions.

Our contributors are already working on creating a Docker image to simplify the setup of self-hosted infrastructure. You can join by following this [discussion](https://github.com/orgs/anyproto/discussions/17) on our GitHub page.

Internally, we're already working on adding network configuration ability into the apps. This will make the process of rebuilding clients optional and greatly simplify the self-hosting flow. We expect to deliver this feature in upcoming releases.



**Custom storage location**

{% hint style="warning" %}
Currently, you can not change the directory of your local data storage. We have it in [plans for Q3 2023](https://github.com/orgs/anyproto/projects/1/views/1). You might consider using a [workaround from our user](https://community.anytype.io/t/custom-storage-location/994) as a temporary solution for Windows and MacOS.
{% endhint %}
