# AnySync Netcheck Tool

A simple tool that checks the ability to connect to Anytype nodes. It was created to test network and TLS (sync) issues.

The _Netcheck_ Tool opens a connection to the coordinator nodes to establish communication with the libp2p protocol and _AnySync_ handshakes, to attempt to execute network configuration requests.

***

### Download <a href="#p-42130-download-2" id="p-42130-download-2"></a>

You can download the version for your OS here:

{% embed url="https://github.com/anyproto/any-sync-tools/releases" %}

The .zip contains all our tools, but the sync check procedure requires only **“any-sync-netcheck”**.\
(The other file is our [self-hosting tool](https://github.com/anyproto/any-sync-tools/blob/main/any-sync-network/README.md).)

### Installation <a href="#p-42130-installation-3" id="p-42130-installation-3"></a>

**Build from source:**

`go install github.com/anyproto/any-sync-tools/any-sync-netcheck@latest`

***

#### Running The Tool <a href="#p-42130-runing-the-tool-5" id="p-42130-runing-the-tool-5"></a>

Execute the file named:

* `any-sync-netcheck`
* _or_ `any-sync-netcheck -v` for a verbose output

***

#### Result <a href="#p-42130-result-6" id="p-42130-result-6"></a>

*   If your sync is **working as expected**, your output log should look something like this:\


    <figure><img src="../../../.gitbook/assets/Screenshot 2023-08-02 at 16.40.02.png" alt=""><figcaption></figcaption></figure>
* **If the tool detects any errors:** please provide all details about your network setup, including VPN, proxy, firewalls, and antivirus. In this event, we may request you to run a trace-route or other system tools for further analysis later on.

***

#### Send to Anyteam <a href="#p-42130-send-to-anyteam-7" id="p-42130-send-to-anyteam-7"></a>

Send the resulting log and your network specs to [support@anytype.io](mailto:support@anytype.io).
