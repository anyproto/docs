# Channel Settings

Channel Settings is where you control everything about a [Channel](../../basics/space.md) — its name and icon, who has access, how notifications behave, what loads first when members enter, and more. There are two ways to get to open the Channel Settings:&#x20;

1. Click the Channel name at the top of the Channel Sidebar.&#x20;
2. Right-click the Channel icon in the Vault Sidebar.&#x20;

<div data-with-frame="true"><figure><img src="../../.gitbook/assets/Docs Channel Settings Intro.jpg" alt=""><figcaption></figcaption></figure></div>

## Preferences

The **General** section covers your Channel's identity and basic behavior.

<div data-with-frame="true"><figure><img src="../../.gitbook/assets/Docs Channel Settings General.jpg" alt=""><figcaption></figcaption></figure></div>

#### Channel name and icon

Your Channel's name and icon are how it appears in everyone's Vault.

* **Icon** — automatically generated during onboarding. To change it, click the icon and choose from the icon library, pick an emoji, or upload your own image.
* **Name** — Hover over the icon area and click **Edit** in the top-right, type the new name, and click **Save**.

#### Homepage

The Homepage is what loads when you (or any member) open the Channel, plus a dedicated **Home** widget is added to your sidebar.

It can be any Object — pick whatever you want members to see first when they enter the Channel.

* **For conversation-focused Channels**, choose a Chat Object as the Homepage so members land in the live discussion.
* **For documentation, wikis, or knowledge Channels**, choose a Page Object — usually a "welcome" or "overview" page that links out to the rest.
* **For project Channels with mixed content**, choose a Collection that brings together everything in scope.
* **Leave it empty** and the last opened Object will load when you re-enter the Channel.

#### Sidebar View

Changes how items in the Sidebar are displayed—either as Widgets or Links. [See more here](../../basics/sidebar/sidebar-widgets.md#widgets-vs.-links).&#x20;

#### Default Object Type

Sets which Object Type is used when you create a new Object without specifying a Type (for example, by pressing Cmd/Ctrl + N or clicking the **+** in the sidebar without choosing).

## Members

Manage who has access to the Channel. Each user is referred to as a Space Member and their access level is determined by their Role. For a more detailed breakdown of shared spaces, please see [collaboration.md](../../collaborate/collaboration.md "mention")

<div data-with-frame="true"><figure><img src="../../.gitbook/assets/Docs Channel Settings Members.jpg" alt=""><figcaption></figcaption></figure></div>

### Roles

There are various roles that Space Member can have, each with different privileges. Be sure to periodically check your members section to ensure everybody has the correct permissions.&#x20;

<table><thead><tr><th width="167.1015625">Role</th><th>Description</th></tr></thead><tbody><tr><td><strong>Viewer</strong></td><td>Can view content in the space but cannot edit documents, chat with others, participate in discussions, or delete anything.</td></tr><tr><td><strong>Editor</strong></td><td>Includes all Viewer privileges, plus the ability to edit content in the space and permanently delete items.</td></tr><tr><td><strong>Admin</strong></td><td>Includes all Editor privileges, plus the ability to manage Editors and Viewers.</td></tr><tr><td><strong>Owner</strong></td><td>Includes all Admin privileges, plus the ability to create Admins, to create invitation links, and transfer channel ownership. </td></tr></tbody></table>

### Access & Invitations

In this section, you are able to invite others into your space and set their permissions. For details on how it works, please see [collaboration.md](../../collaborate/collaboration.md "mention").&#x20;

* Copy link — a shareable URL link for people to join the space.&#x20;
* QR code — A QR code suitable for sharing in public places.&#x20;
* Manage link — settings to restrict and control invitation links.&#x20;
* All — everybody who has access and their role.&#x20;
* Requests — pending requests to join the space that requires approval.&#x20;
* Editors — display only users who are editors.&#x20;
* Viewers — display only users who are viewers.&#x20;

## Notifications

Set the default notification mode for messages in this Channel:

* **Enable all** — every new message produces a notification
* **Mentions only** — only @-mentions trigger notifications
* **Disable all** — no notifications (unread counter still updates, but muted)

Per-Chat and per-Object Discussion settings can override the Channel default.&#x20;

<div data-with-frame="true"><figure><img src="../../.gitbook/assets/Docs Channel Settings Notifications.jpg" alt=""><figcaption></figcaption></figure></div>

## Remote Storage

The Remote Storage tab shows total storage used in this Channel and your remaining storage allowance based on your membership plan. The files listed are specific to the Channel, not your entire Vault.&#x20;

<div data-with-frame="true"><figure><img src="../../.gitbook/assets/Docs Channel Settings Storage.jpg" alt=""><figcaption></figcaption></figure></div>

***

## Content Model

The Content Model tab is the central place to manage your Channel's Types and Properties.

#### Types

A list of every Object Type available in this Channel. From here you can:

* Create new Types
* Edit existing Types — change name, icon, layout, default Properties, Templates
* Configure default behavior per Type

For full details, see [Types](../../organize/types.md).

<div data-with-frame="true"><figure><img src="../../.gitbook/assets/Docs Channel Settings Types.jpg" alt=""><figcaption></figcaption></figure></div>

#### Properties

A list of every Property defined in this Channel. From here you can:

* Create new Properties
* Edit and add new options&#x20;
* See which Types use Property

For full details, see [Properties](../../organize/relations.md).

<div data-with-frame="true"><figure><img src="../../.gitbook/assets/Docs Channel Settings Properties.jpg" alt=""><figcaption></figcaption></figure></div>

***

## Import & Export

The Integrations tab covers everything related to bringing data in and out of the Channel:

* **Import** — bring data in from Notion, Evernote, Obsidian, or generic Markdown / CSV
* **Export** — back up the entire Channel to Markdown or AnyBlock format

<div data-with-frame="true"><figure><img src="../../.gitbook/assets/import.png" alt=""><figcaption></figcaption></figure></div>

***

## Channel Ownership

Channel ownership can be transferred to another member — useful when team roles change, when a creator leaves, or when consolidating responsibilities.

To transfer:

1. Open the Members tab.
2. Click **Transfer ownership** next to the three-dot in the top right corner.
3. Select the future Owner from the list of members.
4. Confirm.

After the transfer:

* The member will become the new Owner.
* You'll become an Editor.
* Only the new Owner can transfer it again.
* The new Owner's membership limits will apply to this channel.

<div data-with-frame="true"><figure><img src="../../.gitbook/assets/Docs Channel Settings Transfer.jpg" alt=""><figcaption></figcaption></figure></div>

## Delete Channel

In shared Channels, only the Owner can delete the Channel. Other members can leave the Channel instead, which removes their access without affecting other members. To delete a Channel:&#x20;

1. Navigate to the General section in your Channel Settings.
2. Click on the 'three dots' button on the top right.
3. Select Delete Channel.&#x20;
4. Enter the name of the Channel to confirm deletion.&#x20;

<div data-with-frame="true"><figure><img src="../../.gitbook/assets/Docs Channel Settings Delete.jpg" alt=""><figcaption></figcaption></figure></div>

{% hint style="danger" %}
**Deleting a Channel is permanent.** All Objects, Chats, Discussions, and history are removed for every member. There is no undo. If you possibly want access to the data later, export the Channel before deleting as precaution.&#x20;
{% endhint %}
