# Networks & Backup

### Anytype Network

Every Anytype user has access to a remote backup node provided by Anytype. Its capacity is currently limited to 1 Gb. Objects and other content have no impact on this limit; only files are limited. If you go over the limit, a warning will appear, and you'll be able to ask for more storage.

Our backup nodes are located in Switzerland.

### **Self-hosted Network**

To backup your spaces and data to a self-hosted network, you need to have a network configuration. If you don’t run your own network yet, see this [how-to guide](https://tech.anytype.io/how-to/self-hosting).

Our contributors are already working on creating a Docker image to simplify the setup of self-hosted infrastructure. You can join by following this [discussion](https://github.com/orgs/anyproto/discussions/17) on our GitHub page.

### Local-only Mode

If you don't want to use any backup solutions at all, you can use our local-only mode. This will disable the backup node completely, and you will only be able to sync between your devices if they are connected to the same local network. Regularly exporting your spaces is recommended if you decide to use this mode since your data is not backed up anywhere.

### Switching Between Networks

We strongly recommend using dedicated identities for each network (local-only mode being the exception). If you are switching from a different network, export all your spaces, and import them into a new identity after switching the network mode.

Please note that all your devices should be manually switched to the same network.

#### Desktop

1. Log out from your current identity.
2. On the onboarding screen, click a gear icon in the top right corner.
3. In the “Network” field pick the network mode you want to use.
4. If you picked the “Self-hosted” mode, upload your self-hosted network configuration (\*.yml file) to the corresponding field.
5. Click the “Save” button.
6. Create a new identity or log in with the existing one.

<figure><img src="../../.gitbook/assets/image (46).png" alt=""><figcaption></figcaption></figure>

#### iOS

1. Log out from your current identity.
2. On the onboarding screen, click a gear icon in the top right corner.
3. Click on the network mode you want to use.
4. If you can't find your network in the list, you can add one by clicking the “Add self-hosted network” button, and choosing your self-hosted network configuration (\*.yml file).
5. Create a new identity or log in with the existing one.

<figure><img src="../../.gitbook/assets/image (48).png" alt="" width="375"><figcaption></figcaption></figure>

#### Android

1. Log out from your current identity.
2. Go to the app settings on the system level (hold the app icon, click “App info”, then go to “Additional app setting”; this flow can differ depending on your Android device).
3. In the “Network” field pick the network mode you want to use.
4. If you picked the “Self-hosted” mode, upload your self-hosted network configuration (\*.yml file) to the corresponding field.
5. Go back to the app.
6. Create a new identity or log in with the existing one.

<figure><img src="../../.gitbook/assets/image (47).png" alt="" width="375"><figcaption></figcaption></figure>
