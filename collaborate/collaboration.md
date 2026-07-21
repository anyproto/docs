# Collaboration

Anytype lets you collaborate with others without sacrificing your privacy.

Unlike traditional cloud apps—where hosting companies can access your content—Anytype uses local-first and end-to-end encryption technology. Your content is always accessible directly on your device and only the people you explicitly invite have the keys to unlock and view it. Anytype’s servers can backup and sync your files, but they never hold the keys to read your content. You can even collaborate directly with others using peer-to-peer sync or self-host on your own network.&#x20;

The result: real collaboration, with no middleman able to see what you're working on.

<div data-with-frame="true"><figure><img src="../.gitbook/assets/Docs Collaborate.gif" alt=""><figcaption></figcaption></figure></div>

## Why it matters

Collaboration in Anytype isn't an afterthought—it's designed from the ground up to give you total ownership and control over your data.

* **Complete Privacy:** Everything in your shared spaces is encrypted _before_ it leaves your device. Only you and your invited teammates can ever read it.
* **Real-Time Sync:** Changes appear instantly when members are online, or on the same local network.
* **Offline-First:** Work freely without an internet connection. Your changes will sync automatically as soon as you're back online.
* **No Sign-Up Hassles:** Collaborators don't need to provide an email address, buy a subscription, or ask anyone for permission. Anyone can set up an Anytype Vault instantly.

This makes shared spaces suitable for sensitive contexts — legal teams, journalists, communities of practice, family planning — anywhere you want collaboration without surveillance.&#x20;

## How it works

With typical cloud apps, your data lives on company servers and is often accessible to third parties like Apple or Google for phone notifications. Anytype does things differently:

1. **Your device holds the keys:** When you create a shared space, your device generates unique encryption keys. These keys are never shared with Anytype or anyone else.
2. **Data is locked before it leaves:** Before your files sync anywhere—whether to Anytype’s servers or another person's phone—they are scrambled into unreadable code.
3. **You pass the keys directly:** When you invite someone, your device securely hands them the decryption key directly with Anytype or anybody else accessing it.&#x20;
4. **Servers act as blind couriers:** Anytype’s servers help sync and back up your data, but because they don't have the keys, all they see is scrambled code.
5. **Unlocking happens only on trusted devices:** The scrambled data is turned back into readable content only when it reaches the devices belonging to the people you invited.

The Bottom Line: Your data is encrypted on your device before it goes anywhere. You and your invited collaborators are the only ones who hold the keys, meaning not even Anytype can read what you're working on.&#x20;

<div><figure><img src="../.gitbook/assets/Docs Regular Sync.gif" alt=""><figcaption><p>Typical Cloud App Sync</p></figcaption></figure> <figure><img src="../.gitbook/assets/Docs E2EE Sync.gif" alt=""><figcaption><p>Anytype Local-first Sync</p></figcaption></figure></div>

## Inviting members

1. Open [Channel Settings](../advanced/settings/space-settings.md) by clicking the Channel name in the Sidebar.&#x20;
2. Click on the Members section.&#x20;

### Invitation Link

The '**Add members via link**' toggle generates a link you can share with others to invite them into the space, either as a text link or a QR code. There are a few important settings to be aware of:

* **Auto Approval** — Enabling this lets users join the space without manual review, which is useful for community or forum-like spaces. For private spaces, it's best to leave this off so every new member requires approval from the Owner.
* **Channel-wide Shareable Invite** — Enabling this allows other members to share the invite link themselves. This works well for public spaces, or private spaces where existing members are highly trusted.
* **Approve Requests** — For members requesting access, you can approve them by navigating to the 'Request' tab which is next to the 'All', 'Editors', and 'Viewers' tab.&#x20;
* **Reset Link** — If you believe an invite link has been compromised, you can reset it. This immediately voids the previous link and generates a new one, which must be used going forward to join the space.

<div data-with-frame="true"><figure><img src="../.gitbook/assets/Docs Invite Link.jpg" alt=""><figcaption></figcaption></figure></div>

{% hint style="danger" %}
**Be sure to share the invitation link with a secure method.** If the invitation link is intercepted, it can be used to gain access to the space. If you are concerned that your invitation links have been compromised, you can reset the link and require request approval for all new joiners.&#x20;
{% endhint %}

### Add Members

The 'add members' button will provide a list of users that you can invite into your space. This list is generated based on users who you are already connected to in other spaces. This is a convenient method to collaborate with people you're already in touch with on Anytype.&#x20;

<div data-with-frame="true"><figure><img src="../.gitbook/assets/Docs Members.jpg" alt=""><figcaption></figcaption></figure></div>

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

**Permanent Delete Permissions**

In shared Channels, Editors can only permanently delete Objects they created, protecting the team from accidental data loss. Owners can permanently delete any Object and can also empty the entire Bin from a single action. This means even if an Editor accidentally clicks "Empty Bin", they can only wipe out their own contributions — nothing of yours or other members' is at risk.

#### Changing access&#x20;

1. Find the Space Member. Use the shortcut `Cmd/Ctrl + F` to search through a large list.&#x20;
2. Click on their current permission level.&#x20;
3. Change it to the desired role. Or remove the member entirely.&#x20;

<div data-with-frame="true"><figure><img src="../.gitbook/assets/Docs Remove Member.jpg" alt=""><figcaption></figcaption></figure></div>

#### Editor seat limits

Each Channel has a maximum number of Editors based on the Owner's plan. The default Free tier supports a small number of Editors per Channel. Higher-tier plans (Builder, Co-Creator, Ultra, Group memberships) increase this limit. See [Memberships](../advanced/monetization/).

Once you reach the limit, new joiners can only join as Viewers until either the limit is raised or an existing Editor is downgraded or removed.

## Joining a Channel

When you receive an invite link, clicking it opens Anytype:

1. If you're not logged in, you'll be prompted to log in or create a Vault.
2. Once logged in, you'll see a confirmation popup with the Channel name and the role you're being given.
3. Click **Accept** to join. The Channel appears in your Vault.

For Request-Access links, the flow is the same except instead of joining immediately, your request goes to the Owner. They'll see a notification and approve or decline; you'll see the Channel appear in your Vault when approved.

## Managing members

From **Channel Settings > Members**, the Owner can:

* **See the list** of all current members with their roles
* **Change a member's role** (Editor ↔ Viewer)
* **Remove a member** entirely (they'll receive a notification and lose access)
* **See pending access requests** for Request-Access invite links
* **Approve or deny** pending requests with a chosen role

#### Members in Chats and Discussions

Member display names and profile pictures (set in their own [Vault Settings > Profile](../advanced/settings/account-and-data.md)) appear next to their messages and posts. Click any member's name or profile to open their profile popup, where you can:

* See their full profile (name, bio, profile picture)
* Send them a Direct Message — opens a [Direct Channel](https://github.com/anyproto/docs-new/blob/main/getting-started/direct-channels.md)
* See which other Channels you both belong to (if any)

## Transferring Channel ownership

Channel ownership can be transferred to another member. Use this when:

* A team lead changes roles
* The original creator leaves the team
* You want to consolidate Owner responsibilities to someone else

#### How to transfer

1. The current Owner opens **Channel Settings > Members**.
2. Click **Transfer ownership** next to the three-dot menu in the top right corner.
3. Select the new Owner from the list of members.
4. Confirm the transfer.

After the transfer:

* The new Owner takes full control, including the ability to transfer ownership again
* You become an Editor (you keep your access but lose Owner-only privileges)

This way, Channels can be handed over as roles change without recreating them or losing history.

## Leaving a Channel

To leave a Channel you've joined:

1. Right-click the Channel in your Vault, **or** open Channel Settings.
2. Click **Leave Channel**.
3. Confirm.

You're removed from the Channel and lose access. Your past contributions (Objects you created, messages you sent) remain in the Channel — Anytype doesn't delete content when a member leaves.

If you're the **Owner**, you can't leave directly — you must first transfer ownership to another member. If there are no other members, you can delete the Channel entirely.

## Real-time sync and offline mode

When all members are online, changes propagate immediately:

* Edit an Object → other members watching the same Object see the change
* Add a Property → it appears in everyone's view of the relevant Type

When members go offline:

* Their changes are queued locally
* When they reconnect, queued changes sync up

## Privacy in shared Channels

Even when sharing, your data stays encrypted:

* **End-to-end encrypted** between members
* **No company access** — Anytype's network nodes hold encrypted data only; they can't decrypt content
* **No log of contents** — what you write, no one outside the Channel can read

For sensitive use, you can also use **self-hosted** networks where you control the relay nodes (see [Networks & Backup](../advanced/data-and-security/self-hosting/)) or **local-only** mode for fully air-gapped sharing on a local network.

## Tips

{% hint style="info" %}
**Use Request-Access links for public-ish Channels.** A community Channel where you want people to find you but want to gate entry works best with Request-Access — the link can be shared widely, but you control who actually gets in.
{% endhint %}

{% hint style="info" %}
**Make a backup before transferring ownership.** Export the Channel (Settings > Integrations > Export Channel) before handing over Owner rights. If anything goes wrong, you have a snapshot.
{% endhint %}

{% hint style="info" %}
**Bring members in as Viewers for review.** If someone needs to read but not edit — for example, a stakeholder reviewing a project — Viewer is exactly right. They see everything, can react to messages, but can't accidentally change anything.
{% endhint %}

{% hint style="warning" %}
**Currently, you can only share entire Channels — not individual Objects.** If you want to share just one thing publicly with no access controls, use [Web Publishing](web-publishing.md) instead.
{% endhint %}

{% hint style="warning" %}
**Once a Channel is deleted, it can't be recovered** unless someone exported it before deletion. Be cautious with **Delete Channel** in shared spaces.
{% endhint %}
