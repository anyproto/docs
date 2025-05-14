# Troubleshooting

If you get an error, you can try these steps before checking the [forum](https://community.anytype.io/) or contacting [support](mailto:support@anytype.io).

1. Ensure that the time on your computer is correct. If the local time is more than 2 hours off, a connection might not be possible.
2. Check if you’re using a proxy, VPN, firewall, or a company network to connect. If yes, try connecting without these to see if it makes a difference.
3. Attempt the connection outside of corporate networks or similar setups.
4. Use your mobile device as a Wi-Fi hotspot for your desktop and try connecting through that.
5. Try to Log in from another device (& network).
6. If you are having graphical issues, try deleting the GPUCache folder under \~/.config/anytype.

For more specific issues:

<details>

<summary>How can I share StackGoroutines log if I'm stuck on login on mobile?</summary>

1. If a hang occurs at StartAccount, you can [tap on Enter My Vault 5 times](https://drive.google.com/file/d/1V4muGfFDNDb98ZVp213-YmbnVv3Vx_tX/view?usp=drive_link).
2. The Rpc.Debug.StackGoroutines command will return a log file.
3. You can share it using any convenient method.

</details>

<details>

<summary>What to do if my storage amount is not properly reflected in the app?</summary>

Navigate to `Debug > Reconcile` in the top menu bar, and restart the app.

</details>

<details>

<summary>What can I do if I don't get asked to choose my anyname after buying a membership?</summary>

Please either type [anytype://main/membership](anytype://main/membership) in your browser or inside Anytype global search, and restart the app.

</details>
