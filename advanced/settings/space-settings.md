# Channel Settings

Channel Settings is where you control everything about a Channel — its name and icon, who has access, how notifications behave, what loads first when members enter, and how Types and Properties are managed. To open Channel Settings:

1. Click the Channel name at the top of the Sidebar. Or right-click the channel icon.
2. Select the option **Channel Settings**.&#x20;

<div data-with-frame="true"><figure><img src="../../.gitbook/assets/Docs Channel Settings.jpg" alt=""><figcaption></figcaption></figure></div>

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

Manage who has access to the Channel. Each user is referred to as a Space Member and their access level is determined by their permissions. It's important to remember to share access to others in a secure method, such as using a private and secure chat.&#x20;

### Roles

There are various roles that Space Member can have, each with different privileges. Be sure to periodically check your members section to ensure everybody has the correct permissions. For a more detailed breakdown, please see [Collaboration](../../collaborate/collaboration.md).&#x20;

<table><thead><tr><th width="167.1015625">Role</th><th>Description</th></tr></thead><tbody><tr><td><strong>Viewer</strong></td><td>Read-only access. Can view content in the space but cannot edit documents, chat with others, participate in discussions, or delete anything.</td></tr><tr><td><strong>Editor</strong></td><td>Includes all Viewer privileges, plus the ability to edit content in the space — including documents, chat, and discussions — and permanently delete items.</td></tr><tr><td><strong>Admin</strong></td><td>Includes all Editor privileges, plus the ability to manage other Space Members' permissions. Can upgrade or downgrade Editors and Viewers, or revoke their access entirely.</td></tr><tr><td><strong>Owner</strong></td><td>Includes all Admin privileges, plus the ability to create Admins, to create invitation links, and transfer channel ownership. </td></tr></tbody></table>

### Inviting others

#### Add Members Button

The 'add members' button will provide a list of users that you can invite into your space. This list is generated based on users who you are already connected to in other spaces.&#x20;

<div data-with-frame="true"><figure><img src="../../.gitbook/assets/Docs Members.jpg" alt=""><figcaption></figcaption></figure></div>

#### Add members via link&#x20;

The '**Add members via link**' toggle generates a link you can share with others to invite them into the space, either as a text link or a QR code. There are a few important settings to be aware of:

* **Auto Approval** — Enabling this lets users join the space without manual review, which is useful for community or forum-like spaces. For private spaces, it's best to leave this off so every new member requires approval from the Owner.
* **Channel-wide Shareable Invite** — Enabling this allows other members to share the invite link themselves. This works well for public spaces, or private spaces where existing members are highly trusted.
* **Approve Requests** — For members requesting access, you can approve them by navigating to the 'Request' tab which is next to the 'All', 'Editors', and 'Viewers' tab.&#x20;
* **Reset Link** — If you believe an invite link has been compromised, you can reset it. This immediately voids the previous link and generates a new one, which must be used going forward to join the space.

<div data-with-frame="true"><figure><img src="../../.gitbook/assets/Docs Invite Link.jpg" alt=""><figcaption></figcaption></figure></div>

### Change access&#x20;

1. Find the Space Member. Use the shortcut `Cmd/Ctrl + F` to search through a large list.&#x20;
2. Click on their current permission level.&#x20;
3. Change it to the desired role. Or remove the member entirely.&#x20;

<div data-with-frame="true"><figure><img src="../../.gitbook/assets/Docs Remove Member.jpg" alt=""><figcaption></figcaption></figure></div>

## Notifications

Set the default notification mode for messages in this Channel:

* **Enable all** — every new message produces a notification
* **Mentions only** — only @-mentions trigger notifications
* **Disable all** — no notifications (unread counter still updates, but muted)

Per-Chat and per-Object Discussion settings can override the Channel default.&#x20;

## Remote Storage

The Remote Storage tab shows total storage used in this Channel and your remaining storage allowance based on your membership plan.

***

## Content Model

The Content Model tab is the central place to manage your Channel's Types and Properties.

#### Types

A list of every Object Type available in this Channel. From here you can:

* Create new Types
* Edit existing Types — change name, icon, layout, default Properties, Templates
* Configure default behavior per Type

For full details, see [Types](../../organize/types.md).

#### Properties

A list of every Property defined in this Channel. From here you can:

* Create new Properties
* Edit and add new options&#x20;
* See which Types use Property

For full details, see [Properties](../../organize/relations.md).

***

## Import & Export

<div data-with-frame="true"><figure><img src="../../.gitbook/assets/import.png" alt=""><figcaption></figcaption></figure></div>

The Integrations tab covers everything related to bringing data in and out of the Channel:

* **Import** — bring data in from Notion, Evernote, Obsidian, or generic Markdown / CSV
* **Export** — back up the entire Channel to Markdown or AnyBlock format

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

<div data-with-frame="true"><figure><img src="../../.gitbook/assets/Transfer Ownership.jpg" alt=""><figcaption></figcaption></figure></div>

## Delete Channel

In shared Channels, only the Owner can delete the Channel. Other members can leave the Channel instead, which removes their access without affecting other members.

<div data-with-frame="true"><figure><img src="../../.gitbook/assets/delete-channel.png" alt=""><figcaption></figcaption></figure></div>

{% hint style="danger" %}
**Deleting a Channel is permanent.** All Objects, Chats, Discussions, and history are removed for every member. There is no undo. If you might want the data later, export the Channel before deleting.&#x20;
{% endhint %}
