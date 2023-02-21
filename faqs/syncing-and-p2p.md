# Syncing & P2P

All your data primarily syncs to the encrypted backup node in the current alpha. For alpha testers, the application is always connected to the backup node and cannot be disconnected.

#### Local backups

Anytype is offline-first, and our backup nodes are still in early testing (we can't guarantee data recovery in 100% cases yet), it may be a good idea to do a regular backup of your Anytype folder (bottom-right question mark → Status → Folder path) to some safe place or with markdown Export.

#### Page history

We have a history of the document changes that you can use if you lose some data and restore previous versions. So the overall risk of losing some data because of the bug is marginal/non-existent. The only part that we can't guarantee is total recovery from our backup node. It's still in testing mode, an Alpha.

### Syncing. How does it work?

All objects are syncing separately. You can have 1 object in the actual state while another is downloading. Every object syncs with all historical changes being merged together. You can work being offline, with different devices different document states.

The app will transfer small chunks (those changes) of data that will build the document back in forth to devices and backup nodes. So when you open the document, not in its actual state. You just need to wait.

Later we will introduce more features bringing transparency into syncing.

### P2P

We transfer objects directly between devices and backup nodes. That means that you can use the app on several devices in one network without connecting to the world wide web. Interconnections trying to establish with all machines being used with time intervals and if connected then checking changes, transfer data online. We can't broadcast every used device every second, so it can take some time to retrieve data from another device (restarting the app can help).

### Status

![](<../.gitbook/assets/Screenshot 2021-11-05 at 16.27.07.png>)

* Status `Synced` is shown when: The app is backed on one node at least. If the app retrieved that no changes were made
* Status `Syncing…` is shown when: For backup node: upload, download, pinning of files. For devices (direct interconnection): upload, download
* Status `No connection` is shown when: Anytype node doesn't connect. You can send the data directly between devices.
* Status `Not syncing` is shown when: The app fails to sync. It can be network problems or bugs.
* Status `Preparing...` is shown when: Warming up and initializing synchronization.

Overall status (for an object):

* If the Object is not fully synced with some device or backup node and something is syncing (like device), → then it is in `Syncing…` state

### Troubleshooting

If you encounter an error during sync:

![](<../.gitbook/assets/image (2).png>)

You will need to send us the «Object diagnostics» for debug. They can be found in the menu bar under the file option. «Object diagnostics» are **confidential**. Please send it to support@anytype.io.

## Future Plans

In the future, we plan on giving users more control over the sync functionality. Some of the features that we are going to implement:

* [ ] Sync Control Options
* [ ] The Precise status of each Object
* [ ] The Naming of Sync Devices
* [ ] Ability to toggle sync for specific pages and objects
