# Troubleshooting

If you get an error, you can try these steps before checking the [forum](https://community.anytype.io/) or contacting [support](mailto:support@anytype.io).

1. Ensure that the time on your computer is correct. If the local time is more than 2 hours off, a connection might not be possible.
2. Check if you’re using a proxy, VPN, firewall, or a company network to connect. If yes, try connecting without these to see if it makes a difference.
3. Attempt the connection outside of corporate networks or similar setups.
4. Use your mobile device as a Wi-Fi hotspot for your desktop and try connecting through that.
5. Try to Log in from another device (& network).
6. For iOS users, check if the sync status turns green. If not, attempt connecting from different networks.
7. If you are having graphical issues, try deleting the GPUCache folder under \~/.config/anytype.

For more specific issues:

<details>

<summary>How can I recover data after a suspected database corruption (Win 11)?</summary>

For the up to date guide on the forum, click [here](https://community.anytype.io/t/how-to-recover-data-in-anytype-on-windows-11-after-a-suspected-database-corruption/12755).

***

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

If after these steps Anytype still doesn’t launch, probably you have spacestore database corrupted. Please take a look at this instructions below.

</details>

<details>

<summary>A tool to fix the 'Anytype Helper Crashed' Issue</summary>

For the up to date guide on the forum, click [here](https://community.anytype.io/t/a-tool-to-fix-the-anytype-helper-crashed-issue/13653).

***

Some Windows users are encountering frequent crashes with the Anytype app, preventing them from accessing their accounts. This issue commonly occurs after unexpected power loss or improper shutdown, leading to database corruption.

The bug will be automatically fixed in the upcoming Anytype update. However, for those who want to address it in the meantime, you can use this tool.

***

### **Instructions to fix the corrupted db:** <a href="#instructions-to-fix-the-corrupted-db-1" id="instructions-to-fix-the-corrupted-db-1"></a>

_For Windows Users_\
**Step 1: Downloading Badger**

* Go to [Release v0.0.4 · anyproto/badger · GitHub 37](https://github.com/anyproto/badger/releases/tag/v0.0.4)
* Download for Windows: Look for the Badger release suitable for Windows.

**Step 2: Accessing PowerShell**

* Open PowerShell: Press Windows Key + X and select “Windows PowerShell” from the menu. Alternatively, you can search for “PowerShell” in the Start menu.

**Step 3: Running Badger**

* Navigate to the Download Folder and open the badger. This will open PowerShell.
* In the PowerShell window, use the `cd` command to change the directory to where you downloaded badger.exe. For example, if it’s in your Downloads folder, you would type cd Downloads.
* Run Badger: Execute the following command:

`.\badger.exe --dir <spacestore_db_path> fix`

* :point\_down: Replace “spacestore\_db\_path” with the actual path to your “Spacestore database”

**Finding the AppData for the “anytype” App:**

The “anytype” app (being an Electron app), stores its data in the AppData folder on your Windows system. To find this:

* Open File Explorer: Press Windows Key + E to open the File Explorer.
* Access AppData: Type %AppData% in the address bar of the File Explorer and press Enter. This will take you to the C:\Users\[YourUsername]\AppData\Roaming folder.
* Locate Anytype Folder: In the Roaming folder, look for a folder named “Anytype”. Inside it you should find “data/” folder. **(If you use beta channel it will be “beta/data/”)**
*   Within this folder you will find “spacestore” folder. You need to copy (ctrl+c) it’s path and put it to the command line mentioned above, replacing “spacestore\_db\_path”.

    The command line it should be something like this:\
    `.\badger.exe --dir C:\Users\Username1\AppData\Roaming\anytype\data\accountId\spacestore`

***

This tool creates the backup of the corrupted db before trying to fix it. Backup will be stored at “spacestore\_corrupted\_backup\_”

***

### When/Who Should Use This Tool: <a href="#whenwho-should-use-this-tool-2" id="whenwho-should-use-this-tool-2"></a>

1. **After Windows BSOD or Power Loss:**

* Use this tool when encountering a Blue Screen of Death (BSOD), loss of access after power outage or improper shutdown on a Windows system.
* Specifically, if the application is not opening and displays an error.

2. **Users in Local-Only Mode with DB Error:**

* Users operating in a local-only mode and encounter a panic error

3. **Users Recovering from Nodes with Data Loss:**

* If users have attempted to recover from nodes, especially with an empty data folder or on another device, and still notice a loss of data (e.g., missing objects or changes)

:octagonal\_sign: **Precaution:** Before Using the Tool: **Remove the “data” Folder**\
The root of the problem may be located in this folder and can be found in the following paths:

_File > Show work directory_ or (`C:\Users\Username1\AppData\Roaming\Anytype`)

* `Anytype/data/<accountID>` for standard release version
* `Anytype/beta/data/<accountID>` folder for _Pre-release_ version
* `Anytype/alpha/data/<accountID>` folder for _Alpha_ (internal) version

</details>

<details>

<summary>How can I share StackGoroutines log if I'm stuck on login on mobile?</summary>

1. If a hang occurs at StartAccount, you can **tap on Enter My Vault 5 times**.
2. The Rpc.Debug.StackGoroutines command will return a log file.
3. You can **share it using any convenient method**.

</details>

