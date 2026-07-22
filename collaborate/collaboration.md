# Collaboration

Anytype lets you collaborate with others without sacrificing your privacy.

Unlike traditional cloud apps—where hosting companies can access your content—Anytype uses local-first and end-to-end encryption technology. Your content is always accessible directly on your device and only the people you explicitly invite have the keys to unlock and view it. Anytype’s servers can backup and sync your files, but they never hold the keys to read your content. You can even collaborate directly with others using peer-to-peer sync or self-host on your own network.&#x20;

The result: real collaboration, with no middleman able to see what you're working on.

<div data-with-frame="true"><figure><img src="../.gitbook/assets/Docs Collaborate.gif" alt=""><figcaption></figcaption></figure></div>

## Why it matters

Collaboration in Anytype isn't an afterthought—it's designed from the ground up to give you total ownership and control over your data.

* **Complete Privacy:** Everything in your shared spaces is encrypted _before_ it leaves your device. Only you and your invited teammates can ever read it.
* **Real-Time Sync:** Changes appear instantly when members are online, or on the same local network.
* **Offline-First:** Work freely without an internet connection. Your changes will sync automatically as soon as you establish a network connection, which can be peer-to-peer.&#x20;
* **No Sign-Up Hassles:** Collaborators don't need to provide an email address, buy a subscription, or ask anyone for permission. Anyone can set up an Anytype Vault instantly.

This makes shared spaces suitable for sensitive contexts — legal teams, journalists, communities of practice, family planning — anywhere you want collaboration without surveillance.&#x20;

## How it works

With typical cloud apps, your data lives on company servers and is often accessible to third parties like Apple or Google for phone notifications. Anytype does things differently:

1. **Your device holds the keys:** When you create a shared space, your device generates unique encryption keys. These keys are never shared with Anytype or anyone else.
2. **Data is encrypted before it leaves:** Before your files sync anywhere—whether to Anytype’s servers or another person's phone—they are scrambled into unreadable code.
3. **You pass the keys directly:** When you invite someone to a space, your device securely hands them the decryption key directly without Anytype or anybody else accessing it.&#x20;
4. **Servers act as blind couriers:** Anytype’s servers help sync and back up your data, but because they don't have the keys, all they see is scrambled code.
5. **Unlocking happens only on trusted devices:** The scrambled data is turned back into readable content only when it reaches the devices belonging to the people you invited.

The Bottom Line: Your data is encrypted on your device before it goes anywhere. You and your invited collaborators are the only ones who hold the keys, meaning not even Anytype can read what you're working on.&#x20;

<div><figure><img src="../.gitbook/assets/Docs Regular Sync.gif" alt=""><figcaption><p>Typical Cloud App Sync</p></figcaption></figure> <figure><img src="../.gitbook/assets/Docs E2EE Sync.gif" alt=""><figcaption><p>Anytype Local-first Sync</p></figcaption></figure></div>

## Joining Channels

When you receive an invite link, clicking it opens Anytype:

1. If you're not logged in, you'll be prompted to log in or create a Vault.
2. Once logged in, you'll see a confirmation popup with the Channel and the role you're given.
3. Click **Accept** to join. The Channel appears in your Vault.

For Request-Access links, the flow is the same except instead of joining immediately, your request goes to the Owner. They'll see a notification and approve or decline; you'll see the Channel appear in your Vault when approved.

## Inviting members

1. Open [Channel Settings](../advanced/settings/space-settings.md) by clicking the Channel name in the Sidebar.&#x20;
2. Click on the Members section.&#x20;
3. Choose your invitation method — availability is set by the Space Owner.&#x20;

<div data-with-frame="true"><figure><img src="../.gitbook/assets/Docs Collaborate Invite.jpg" alt=""><figcaption></figcaption></figure></div>

### Invitation Link

The '**Add members via link**' toggle generates a link you can share with others to invite them into the space, either as a text link or a QR code. There are a few important settings to be aware of:

* **Enable auto approval** — Enabling this lets users join the space without manual review, which is useful for community or forum-like spaces. For private spaces, it's best to leave this off so every new member requires approval from the Owner.
* **Everyone in the channel can share this invite** — Enabling this allows other members to share the invite link themselves. This works well for public spaces without sensitive data or private spaces where existing members are highly trusted.
* **Reset Link** — If you believe an invite link has been compromised, you can reset it. This immediately voids the previous link and generates a new one, which must be used going forward to join the space.
* **Approve Requests** — For members requesting access, you can approve them by navigating to the 'Request' tab which is next to the 'All', 'Editors', and 'Viewers' tab.&#x20;

<div data-with-frame="true"><figure><img src="../.gitbook/assets/Docs Invite Link.jpg" alt=""><figcaption></figcaption></figure></div>

{% hint style="danger" %}
**Be sure to share auto-approve invitation links with a secure method.** If it is intercepted, it can be used to gain access to the space without approval. If you are concerned that your invitation links have been compromised, you can reset the link and require request approval for all new joiners.&#x20;
{% endhint %}

### Add Members

The 'add members' button will provide a list of users that you can invite into your space. This list is generated based on users who you are already connected to in other spaces. This is a convenient method to collaborate with people you're already in touch with on Anytype without needing to send an invitation link separately.&#x20;

<div data-with-frame="true"><figure><img src="../.gitbook/assets/Docs Collaborate Add.jpg" alt=""><figcaption></figcaption></figure></div>

{% hint style="info" %}
**If there are many unrecognisable users in your member list**, this may be due to you being part of a community space with many other members not recognizable to you.&#x20;
{% endhint %}

## Member roles

Every Channel has multiple role levels:

| Role       | Create, edit, and remove Objects | Chat & Discussions | Edit Channel name/icon | Pin Objects to Sidebar |       Permanent delete      |      Manage members      |
| ---------- | :------------------------------: | :----------------: | :--------------------: | :--------------------: | :-------------------------: | :----------------------: |
| **Owner**  |                 ✓                |          ✓         |            ✓           |            ✓           | All Objects (incl. others') |             ✓            |
| **Admin**  |                 ✓                |          ✓         |            ✓           |            ✓           | All Objects (incl. others') | Only editors and viewers |
| **Editor** |                 ✓                |          ✓         |           ✓            |            —           |        Only their own       |             —            |
| **Viewer** |                —                 |          —         |            —           |            —           |              —              |             —            |

#### Permanent delete permissions

In shared Channels, Editors can only permanently delete Objects they created, protecting the team from accidental data loss. Owners can permanently delete any Object and can also empty the entire Bin from a single action. This means even if an Editor accidentally clicks "Empty Bin", they can only wipe out their own contributions — nothing of yours or other members' is at risk.

#### Editor seat limits

Each Channel has a maximum number of Editors based on the Owner's plan. The default Free tier supports a small number of Editors per Channel. Higher-tier plans (Builder, Co-Creator, Ultra, Group memberships) increase this limit. See [Memberships](../advanced/monetization/).

Once you reach the limit, new joiners can only join as Viewers until either the limit is raised or an existing Editor is downgraded or removed.

## Managing members

From the members section, the Owner and Admin can:

* **See the list** of all current members with their roles.
* **Approve or deny** pending requests for users asking to join the space.
* **Change a member's role** such as upgrading a Viewer to an Editor.&#x20;
* **Remove a member** where they'll receive a notification and lose access.&#x20;
* **Search the member list** using the shortcut `Cmd/Ctrl + F`&#x20;

#### Changing access&#x20;

* Find the Space Member.&#x20;
* Click on their current permission level.&#x20;
* Change it to the desired role. Or remove the member entirely.&#x20;

<div data-with-frame="true"><figure><img src="../.gitbook/assets/Docs Remove Member.jpg" alt=""><figcaption></figcaption></figure></div>

#### Members in Chats and Discussions

Member display names and profile pictures appear next to their messages and posts. Click any member's name or profile to:

* See their full profile — name, bio, profile picture
* Connect with them — opens a [Direct Channel](https://github.com/anyproto/docs-new/blob/main/getting-started/direct-channels.md)

<div data-with-frame="true"><figure><img src="../.gitbook/assets/Docs Direc Channel Connect.jpg" alt=""><figcaption></figcaption></figure></div>

## Transfer ownership

Channel ownership can be transferred to another member in the [Channel Settings](../advanced/settings/space-settings.md#channel-ownership).&#x20;

## Leaving a Channel

To leave a Channel you've joined:

1. Right-click the Channel in your Vault, or open Channel Settings.
2. Click **Leave Channel**.
3. Confirm.

Your past contributions remain in the Channel after leaving it — Anytype does not remove your chat messages or documents in a space, you must delete them before leaving.&#x20;

<div data-with-frame="true"><figure><img src="../.gitbook/assets/Docs Collaborate Leave Channel.jpg" alt=""><figcaption></figcaption></figure></div>

{% hint style="warning" %}
**Owners of a space must first transfer ownership to another member.** If there are no other members, you can delete the Channel entirely.
{% endhint %}

## Syncing offline

When members are **online**, changes update immediately like usual:

* Make an edit → other members will see the change in real-time.&#x20;
* Send a message → it appears in the Chat straight away.&#x20;

When members are **offline**, everything still works by default:&#x20;

* Make an edit → it will save locally and be queued for sync once back online.&#x20;
* Send a message → it appears locally but will only be sent once back online.&#x20;

Anytype is built with local-first technology, which means that everything works offline by default and syncs with end-to-end encryption again once a network connection is established.&#x20;

## Privacy in shared Channels

When sharing spaces and collaborating with others on Anytype, your data stays encrypted when being synced. For even more sensitive and high security cases, you can also use **self-hosted** networks where you control the relay nodes (see [Networks & Backup](../advanced/data-and-security/self-hosting/)) or **local-only** mode for fully air-gapped sharing on a local network.&#x20;

## Tips

{% hint style="info" %}
**Use Request-Access invitation links for more control.** Auto-approval invitation links should only be used in spaces where quick and easy access takes priority over protecting sensitive data.&#x20;
{% endhint %}

{% hint style="info" %}
**Make a backup before transferring ownership.** Export the Channel (Settings > Integrations > Export Channel) before handing over Owner rights. If anything goes wrong, you have a snapshot.
{% endhint %}

{% hint style="warning" %}
**Currently, you can only share entire Channels — not individual Objects.** If you want to share just one thing publicly with no access controls, use [Web Publishing](web-publishing.md) instead.
{% endhint %}

{% hint style="warning" %}
**Once a Channel is deleted, it can't be recovered** unless someone exported it before deletion. Be cautious with Delete Channel in shared spaces.&#x20;
{% endhint %}
