---
description: Real-time conversations alongside your work.
---

# Chats

A **Chat** is a real-time conversation thread inside a Channel. Unlike messages in a separate app, Chats live alongside your notes, tasks, and documents — discussions stay private, encrypted, and contextually linked to the work they're about.

Chats give you the rhythm of a messaging app — quick replies, reactions, file shares — but with a twist: every message can reference, create, or open Anytype Objects. A typed thought becomes a Page; a screenshot becomes a File Object; a question can be answered with an Object link that opens in a click.

<div data-with-frame="true"><figure><img src="../../.gitbook/assets/Docs Chat Launch.jpg" alt=""><figcaption></figcaption></figure></div>

## How it works

Just like documents and files, Chats are [Objects](../../creation/objects/) that have their own dedicated [Type](../../organize/types.md). This means that a Chat:

* Lives in the Types section of the Sidebar under 'Chat'.
* Can have its own [Properties](../../organize/properties.md).
* Can be organized into [Views](../../organize/views.md), [Queries](../../organize/queries.md), and [Collections](../../organize/collections.md).
* Can be added as a [Widget](../../basics/sidebar/widgets.md) to the Sidebar.
* Can be `@`-mentioned or linked like any other Object.

Chat is a system Type, so it doesn't support custom Templates or layout changes. But everything else about Chat behaves like a regular Object Type.

## Creating Chats

#### Single Chat

1. In the Channel Sidebar header, click on the create dropdown.
2. Select Chat from the list of Types.
3. Give the Chat a name.

<div data-with-frame="true"><figure><img src="../../.gitbook/assets/Docs Chat Create.jpg" alt=""><figcaption></figcaption></figure></div>

{% hint style="info" %}
**Set a Chat as the home page** for Channels where conversations take the forefront.
{% endhint %}

#### Multiple Chats

A single Channel can hold multiple Chats. You can start topic-specific conversations right where the work happens and keep them organized by using [Views](../../organize/views.md).

1. Navigate to Chats in the Types section in the Sidebar.
2. Create a new Chat.
3. Add your desired Properties.
4. Set your preferred Filters and Sorts.
5. Set your desired Layout.

<div data-with-frame="true"><figure><img src="../../.gitbook/assets/Docs Chats Multiple.jpg" alt=""><figcaption></figcaption></figure></div>

{% hint style="info" %}
**Use multiple Chats for large Channels.** A single team Channel can have multiple Chats. Mute the noisy ones, leave Mentions-only on others.
{% endhint %}

#### Chats Widget

The Chats Widget works like any other widget in your sidebar:

* Pin it to keep it always visible
* Adjust its appearance (compact, list, etc.)

<div data-with-frame="true"><figure><img src="../../.gitbook/assets/Docs Chat Widget.jpg" alt=""><figcaption></figcaption></figure></div>

{% hint style="info" %}
**Group your Chats into categories and use a Kanban board layout** to create an organized list in your Sidebar.
{% endhint %}

## Using Chat

#### Sending messages

The message input lives at the bottom of every Chat. You can send:

* **Text** — typed inline, with full markdown formatting
* **Mentions** — `@` to mention a member or any Object
* **Attachments** — drag in a file, paste an image, or share an Object using the 'plus' button.

<div data-with-frame="true"><figure><img src="../../.gitbook/assets/Docs Chats Using.jpg" alt=""><figcaption></figcaption></figure></div>

#### Reactions

Hover over any message and click the smiley icon to react with an emoji.

When more than one person reacts with the same emoji, you'll see a counter next to that reaction. Click the reaction to add or remove your own.

#### Replies

Right-click a message (or hover and click the reply icon) to reply to it specifically. Your reply quotes the original at the top — recipients see the context immediately and can click the quoted preview to **jump to the original message**.

The scroll-down button takes you back to the reply first, then to the bottom of the chat — so you can navigate replies without losing your place.

#### Smart Anytype links

When you paste an Anytype Object link into the Chat message box, it automatically converts into an attachment card. This means recipients see a rich preview of the Object instead of a long URL string.

#### Pinning messages

You can pin important messages in a Chat:

1. Right-click the message.
2. Choose **Pin**.

Pinned messages appear in a **persistent banner at the top of the conversation**. When multiple messages are pinned, click the banner to cycle through them from newest to oldest.

#### Chat message search

Search inside the active Chat with **Cmd/Ctrl + F** (or click the search icon at the top of the Chat). Results appear in a dropdown sorted by date, with navigation arrows to move through matches one by one.

For Channel-wide search across all Chats and Objects, use the global search (Cmd/Ctrl + K from anywhere).

#### Editing and deleting messages

Right-click your own message (or hover and use the three-dot menu) to:

* **Edit** — message stays in place but is marked as edited
* **Copy text** — copy the message content (with formatting preserved)
* **Delete** — remove the message entirely

You can only edit or delete your own messages. Channel Owners cannot edit other members' messages.

#### File attachments

Drag a file onto the Chat input or paste it from the clipboard. The file uploads and:

* Becomes a [File Object](https://github.com/anyproto/docs-new/blob/main/getting-started/files-and-media.md) you can find later
* Shows as a preview card in the chat
* Is searchable through global search

For images, the message includes a preview thumbnail. Audio and video include an inline player.

## Chat Notifications

#### Unread section

A temporary **Unread** section appears automatically when new messages arrive in any Chat. As you catch up, the section shrinks and eventually disappears. This section also displays notifications from [Discussions](../discussions.md). Learn more in the [Sidebar](../../basics/sidebar/sections.md) section.

<div data-with-frame="true"><figure><img src="../../.gitbook/assets/Docs Chats Unread.jpg" alt=""><figcaption></figcaption></figure></div>

#### Per-chat Notifications

Per-Chat notification settings let you control how loud each Chat is.

1. Open your desired Chat.
2. Click the three-dot button in the top right corner.
3. Select **Notifications**.
4. Choose:
   * **Enable all** — notifications for every message
   * **Mentions only** — only when you're `@`-mentioned
   * **Disable all** — no notifications (unread counter still updates)

These settings are per-Chat and override Channel-level defaults. See [Notifications](https://github.com/anyproto/docs-new/blob/main/getting-started/notifications.md) for the full picture.

## Chat Settings

#### Chat as a Channel Home

When you create a Channel, you can choose **Chat** as the Home — meaning the first thing anyone sees when they open the Channel is the live conversation. Chat-Home Channels are great for:

* Team standups and async chat
* Communities and interest groups
* Work where conversation is primary, with documents as supporting cast

See [Channels](../../basics/channels.md#choosing-a-home) for more details.

<div data-with-frame="true"><figure><img src="../../.gitbook/assets/home-chat.png" alt=""><figcaption></figcaption></figure></div>

#### Send message preference

Choose how messages are sent in **Vault Settings > Application > Preferences > Messaging**.

* **Enter** to send (Shift + Enter for a new line)
* **Cmd / Ctrl + Enter** to send (Enter for a new line)

#### Spell checking

Chat messages support spell checking with the same red underline and suggestions as the editor. It uses your existing language settings — no extra setup needed. Configure spellcheck languages in **Vault Settings > Application > Language & Region**.

## Direct Channels

For one-on-one conversations with others, use **Direct Channels** — private chats between two people, with no admin or hierarchy. See [Direct Channels](direct-channels.md) for more information.

## Exporting Chats

You cannot export a chat from a Channel. Chat messages are tied to the individual members of a space, and each member's data is secured with unique encryption keys. When you export a space and import it into a new one, that new space is created with entirely different encryption keys and members.

As a result, chat objects and messages cannot be exported — they are inherently bound to the space in which they were created.

## Tips

{% hint style="info" %}
**Drop Objects into Chat to share work in progress** — Note, Task, Page, even another Chat. The Object becomes a clickable attachment card. Recipients can open and edit immediately.
{% endhint %}

{% hint style="info" %}
**Pin the welcome message.** When someone joins a Channel, the first thing they see is the pinned message at the top. Use this to set norms — what the Channel is for, how to engage.
{% endhint %}

{% hint style="info" %}
**For Object-specific feedback, use Discussions instead of Chat.** Discussions live on the Object and stay attached forever. Chats are for cross-Object conversations and stream-of-consciousness collaboration. See [Discussions](https://github.com/anyproto/docs-new/blob/main/getting-started/discussions.md).
{% endhint %}
