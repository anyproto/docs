# Troubleshooting

If you get an error, you can try these steps before checking the [forum](https://community.anytype.io/) or contacting [support](mailto:support@anytype.io).

1. Ensure that the time on your computer is correct. If the local time is more than 2 hours off, a connection might not be possible.
2. Check if you’re using a proxy, VPN, firewall, or a company network to connect. If yes, try connecting without these to see if it makes a difference.
3. Attempt the connection outside of corporate networks or similar setups.
4. Use your mobile device as a Wi-Fi hotspot for your desktop and try connecting through that.
5. Try to Log in from another device (& network)
6. For iOS users, check if the sync status turns green. If not, attempt connecting from different networks.
7. If you are having graphical issues, try deleting the GPUCache folder under \~/.config/anytype.

### How to Recover Data After a Suspected Database Corruption (Win 11)

If you’re experiencing issues with Anytype, such as after a sudden power loss, and suspect database corruption, follow these step-by-step instructions to recover your data:

**Step 1**: Locate the Anytype Account Data

1. Open File Explorer: Press `Win + E` to open File Explorer.
2. Access the AppData Folder: In the address bar, type `%AppData%` and press `Enter`. This takes you to the `Roaming` folder inside `AppData`.
3. Navigate to Anytype Data Folder: Go to the Anytype folder by following this path:
4. `Anytype > data > <accountId>` or `Anytype > beta > data > <accountId>` in case you are on the Pre-release(beta) channel in anytype
5. Replace `<accountId>` with your specific account ID.

**Step 2:** Rename the Localstore Database

1. Find the Localstore Folder: Inside the Anytype data folder, look for a folder named `localstore`.
2. Rename the Localstore Folder: Right-click on the `localstore` folder and select `Rename`. Change the name to something like `localstore_backup`. This step ensures that Anytype will create a new localstore database when it runs next, while keeping your old data safe in the renamed folder.

**Step 3:** Restart Anytype

1. Launch Anytype: Open the Anytype application on your computer.
2. Check for Normal Operation: Anytype should now launch without issues. It will create a new localstore database automatically.

If after these steps Anytype still doesn’t launch, probably you have spacestore database corrupted. Please take a look at this instruction [A tool to fix the 'Anytype Helper Crashed' Issue 2](https://community.anytype.io/t/a-tool-to-fix-the-anytype-helper-crashed-issue/13653).
