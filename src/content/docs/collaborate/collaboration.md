---
title: "Collaboration"
---

Anytype lets you collaborate with others without sacrificing your privacy.

Unlike traditional cloud apps—where hosting companies can access your content—Anytype uses local-first and end-to-end encryption technology. Your content is always accessible directly on your device, and only the people you explicitly invite have the keys to unlock and view it. Anytype’s servers can back up and sync your files, but they never hold the keys to read your content. You can even collaborate directly with others using peer-to-peer sync or self-host on your own network.

The result: real collaboration, with no middleman able to see what you're working on.

![docs collaborate](/assets/docs-collaborate.gif)

## Why it matters

Collaboration in Anytype isn't an afterthought—it's designed from the ground up to give you total ownership and control over your data.

* **Complete Privacy:** Everything in your shared spaces is encrypted _before_ it leaves your device. Only you and your invited teammates can ever read it.
* **Real-Time Sync:** Changes appear instantly when members are online, or on the same local network.
* **Offline-First:** Work freely without an internet connection. Your changes will sync automatically as soon as you establish a network connection, which can be peer-to-peer.
* **No Sign-Up Hassles:** Collaborators don't need to provide an email address, buy a subscription, or ask anyone for permission. Anyone can set up an Anytype Vault instantly.

This makes shared spaces suitable for sensitive contexts — legal teams, journalists, communities of practice, family planning — anywhere you want collaboration without surveillance.

## How it works

With typical cloud apps, your data lives on company servers and is often accessible to third parties like Apple or Google for phone notifications. Anytype does things differently:

1. **Your device holds the keys:** When you create a shared space, your device generates unique encryption keys. These keys are never shared with Anytype or anyone else.
2. **Data is encrypted before it leaves:** Before your files sync anywhere—whether to Anytype’s servers or another person's phone—they are scrambled into unreadable code.
3. **You pass the keys directly:** When you invite someone to a space, your device securely hands them the decryption key directly without Anytype or anybody else accessing it.
4. **Servers act as blind couriers:** Anytype’s servers help sync and back up your data, but because they don't have the keys, all they see is scrambled code.
5. **Unlocking happens only on trusted devices:** The scrambled data is turned back into readable content only when it reaches the devices belonging to the people you invited.

The Bottom Line: Your data is encrypted on your device before it goes anywhere. You and your invited collaborators are the only ones who hold the keys, meaning not even Anytype can read what you're working on.

![Typical Cloud App Sync](/assets/docs-regular-sync.gif)
_Typical Cloud App Sync_![Anytype Local-first Sync](/assets/docs-e2ee-sync.gif)
_Anytype Local-first Sync_

## Inviting and joining

1. Open [Channel Settings](/settings/channel-settings/) by clicking the Channel name in the Sidebar.
2. Click on the Members section.
3. Choose your invitation method — availability is set by the Space Owner.

![docs collaborate invite](/assets/docs-collaborate-invite.jpg)

### Invitation Link

The '**Add members via link**' toggle generates a link you can share with others to invite them into the space, either as a text link or a QR code. By default, all requests to join the space require approval. There are a few important settings to be aware of:

* **Enable auto approval** — This lets users join the space automatically without manual review, which is useful for community or forum-like spaces. For private and sensitive spaces, it's best to not enable this.
* **Everyone in the channel can share this invite** — Enabling this allows other members to share the invite link themselves. This works well for public spaces without sensitive data or private spaces where members are highly trusted.
* **Reset Link** — If you believe an invite link has been compromised, you can reset it. This immediately voids the previous link and generates a new one, which must be used going forward to join the space.
* **Approve Requests** — For members requesting access, approve them from the 'Requests' tab, next to the 'All', 'Editors', and 'Viewers' tabs.

![docs invite link](/assets/docs-invite-link.jpg)

:::danger
**Be sure to share auto-approve invitation links with a secure method.** If it is intercepted, it can be used to gain access to the space without approval. If you are concerned that your invitation links have been compromised, you can reset the link and require request approval for all new joiners.
:::

### Add Members

The 'add members' button will provide a list of users that you can invite into your space. This list is generated based on users who you are already connected to in other spaces. This is a convenient method to collaborate with people you're already in touch with on Anytype without needing to send an invitation link separately.

![docs collaborate add](/assets/docs-collaborate-add.jpg)

:::note
**If there are many unrecognisable users in your member list**, this may be due to you being part of a large community space with many members unrecognizable to you.
:::

### Joining Channels

When you receive an invite link, clicking it opens Anytype:

1. If you're not logged in, you'll be prompted to log in or create a Vault.
2. Once logged in, you'll see a confirmation popup with the Channel and the role you're given.
3. Click **Accept** to join. The Channel appears in your Vault.

For Request-Access links, the flow is the same except instead of joining immediately, your request goes to the Owner. They'll see a notification and approve or decline; you'll see the Channel appear in your Vault when approved.

## Members

All members who are part of a space are referred to as Space Members. You can be referenced with `@` mentions, assigned tasks, and participate in discussions.

### Roles

All spaces have multiple role levels, each with progressively higher privileges: Viewer, Editor, Admin, and Owner. In short:

* **Viewers** can only read content.
* **Editors** can edit and delete.
* **Admins** can manage members.
* **Owners** can do everything.

<table data-search="false"><thead><tr><th>Privilege</th><th width="102.04296875" align="center">Viewer</th><th width="104.13671875" align="center">Editor</th><th width="108.62109375" align="center">Admin</th><th width="108.6015625" align="center">Owner</th></tr></thead><tbody><tr><td>Create, edit, and remove objects</td><td align="center">—</td><td align="center">✓</td><td align="center">✓</td><td align="center">✓</td></tr><tr><td>Participate in chats &#x26; discussions</td><td align="center">—</td><td align="center">✓</td><td align="center">✓</td><td align="center">✓</td></tr><tr><td>Edit space name &#x26; icon</td><td align="center">—</td><td align="center">✓</td><td align="center">✓</td><td align="center">✓</td></tr><tr><td>Add shared pins to sidebar</td><td align="center">—</td><td align="center">—</td><td align="center">✓</td><td align="center">✓</td></tr><tr><td>Manage members</td><td align="center">—</td><td align="center">—</td><td align="center">Editors &#x26; viewers</td><td align="center">✓</td></tr><tr><td>Manage invitation links</td><td align="center">—</td><td align="center">—</td><td align="center">—</td><td align="center">✓</td></tr><tr><td>Change space ownership</td><td align="center">—</td><td align="center">—</td><td align="center">—</td><td align="center">✓</td></tr></tbody></table>

:::note
**To share an Object with somebody outside of Anytype**, use the publish feature. This creates a webpage that can be visited in the browser.
:::

:::caution
**You cannot set permissions on a per-Object basis.** All Space Members can view everything inside a Space. If you require more separation, use a different space and import only the content you are happy to share with everyone.
:::

### Managing members

From the members section, the Owner and Admin can:

* **See the list** of all current members with their roles.
* **Approve or deny** pending requests for users asking to join the space.
* **Change a member's role** such as upgrading a Viewer to an Editor.
* **Remove a member** where they'll receive a notification and lose access.
* **Search the member list** using the shortcut `Cmd/Ctrl + F`

#### Changing access

* Find the Space Member.
* Click on their current permission level.
* Change it to the desired role. Or remove the member entirely.

![docs remove member](/assets/docs-remove-member.jpg)

#### Editor seat limits

Each Channel has a maximum number of Editors based on the Owner's plan. The default Free tier supports a small number of Editors per Channel. Higher-tier plans (Builder, Co-Creator, Ultra, Group memberships) increase this limit. See [Memberships](../resources/memberships/).

Once you reach the limit, new joiners can only join as Viewers until either the limit is raised or an existing Editor is downgraded or removed.

## Collaborating with others

#### Working and syncing offline

Anytype is built with local-first technology, which means that everything works offline by default and syncs with end-to-end encryption again once a network connection is established. You don't need to save specific pages for offline use.

When members are **online**, changes update immediately like usual:

* Make an edit → other members will see the change in real-time.
* Send a message → it appears in the Chat straight away.

When members are **offline**, everything still works by default:

* Make an edit → it will save locally and be queued for sync once back online.
* Send a message → it appears locally but will only be sent once back online.

#### Members in Chats and Discussions

Member names and profile pictures appear next to their messages and posts. Click any member's name or profile to:

* See their full profile — name, bio, profile picture
* Connect with them privately — opens a [Direct Channel](https://github.com/anyproto/docs-new/blob/main/getting-started/direct-channels.md)

![docs direc channel connect](/assets/docs-direc-channel-connect.jpg)

#### Privacy in shared Channels

When sharing spaces and collaborating with others on Anytype, your data stays encrypted during sync. You can collaborate with peace of mind. However, only share spaces with people you trust. They can view and export data.

For more sensitive, high-security cases, use **self-hosted** networks where you control the relay nodes. See [Networks & Backup](../data/sync-and-backup/). You can also use **local-only** mode for fully air-gapped sharing on a local network.

## Leaving a Channel

To leave a Channel you've joined:

1. Right-click the Channel in your Vault, or open Channel Settings.
2. Click **Leave Channel**.
3. Confirm.

Your past contributions remain in the Channel after leaving it — Anytype does not remove your chat messages or documents in a space.

![docs collaborate leave channel](/assets/docs-collaborate-leave-channel.jpg)

:::caution
**Owners of a space must first transfer ownership to another member before leaving.** If there are no other members, you can delete the Channel entirely.
:::

## Tips

:::note
**Use Request-Access invitation links for more control.** Auto-approval invitation links should only be used in spaces where quick and easy access takes priority over protecting sensitive data.
:::

:::note
**Make a backup before transferring ownership.** Export the Channel (Settings > Integrations > Export Channel) before handing over Owner rights. If anything goes wrong, you have a snapshot.
:::

:::caution
**Currently, you can only share entire Channels — not individual Objects.** If you want to share just one thing publicly with no access controls, use [Web Publishing](/collaborate/publish/) instead.
:::

:::caution
**Once a Channel is deleted, it can't be recovered** unless someone exported it before deletion. Be cautious with Delete Channel in shared spaces.
:::
