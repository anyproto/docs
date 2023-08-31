# Backup & Self-Hosting

## Backup node

Every Anytype user has access to a remote backup node provided by Anytype. Its capacity is currently limited to 1 Gb. If you go over the limit, a warning will appear, and you'll be able to ask for more storage. Our backup nodes are located in Switzerland.

We plan on introducing third party sync providers in the future.

#### Disable the Anytype backup node

There is currently no option in the account settings to disable the backup node, but this is something we are planning on [introducing soon](https://github.com/anyproto/roadmap/issues/34) (**2023Q3**).

Alternatively, you can [block Anytype network traffic](https://community.anytype.io/t/is-there-a-way-to-limit-storage-of-data-only-local/6982) (Anytype & Anytype Helper) via your firewall.

## **How to self-host Anytype**

If you don’t want to use Anytype backup node, you can self-host your own using [this guide](https://tech.anytype.io/how-to/self-hosting). It is our first step in this direction, so it requires some technical skills from users and depends on several external solutions.

Our contributors are already working on creating a Docker image to simplify the setup of self-hosted infrastructure. You can join by following this [discussion](https://github.com/orgs/anyproto/discussions/17) on our GitHub page.

Internally, we're already working on adding network configuration ability into the apps. This will make the process of rebuilding clients optional and greatly simplify the self-hosting flow. We expect to deliver this feature in upcoming releases.
