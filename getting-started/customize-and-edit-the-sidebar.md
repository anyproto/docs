---
description: How to navigate, customize, and organize the Channel sidebar.
---

# Sidebar

### What is the Sidebar?

The **Sidebar** is the main navigation panel for a Channel. It lives on the left side of the window, between your Vault (the leftmost narrow panel showing all Channels) and your editor.

The Sidebar is the entry point to almost everything inside a Channel:

* A **Channel header** at the top with the Channel's name, search, settings, and members
* **Pinned and Favorite** sections for quick access
* **Recently Edited** for catching up
* **The Types section** showing every Object grouped by Type
* The **Bin** for deleted Objects

Everything you do in a Channel either starts here or returns here.

### Layout overview

#### Channel sidebar header

At the very top, you'll see your Channel name and icon, plus icons for:

* **Members** — see who's in the Channel and their roles
* **Channel's Menu** (the drop-down arrow) — access to Channel Settings and Manage Sections in your sidebar
* **Search** (Cmd/Ctrl + K from anywhere) — find any Object in this Channel
* **Create New Object** (Cmd/Ctrl + N) — instantly add a new Default Object

#### Section list

Below the header, sections appear in this order by default (you can reorder):

1. **Shared Pins** — Objects pinned by the Owner for everyone
2. **Unread** — A temporary section with notifications (new messages, replies)
3. **My Favorites** — your personal favorites
4. **Recently Edited** — Objects modified recently
5. **Types** — all Objects in the Channel grouped by Type
6. **Bin** — deleted Objects awaiting permanent deletion

Each section can be hidden, reordered, or fine-tuned. See [Manage Sidebar Sections](manage-sidebar-sections.md) for details.

### Pinning and Favoriting

Anytype has two distinct mechanisms:

* **My Favorites** — personal, visible only to you, on every device you log into
* **Shared Pins** — public, visible to all members (Owner-only to add)

These appear as separate sections in the sidebar. See [Pins & Favorites](pins-and-favorites.md) for the full breakdown.

#### To favorite or pin an Object

1. Open the Object.
2. Click the star (favorite) or pin icon in the top-right corner of the editor.
3. The Object appears in the corresponding sidebar section.

To remove, click the icon again or right-click the item in the sidebar and choose **Remove from Favorites** / **Unpin**.

### Recently Edited

The **Recently Edited** section shows Objects that have been modified recently — useful for picking up where you (or your team) left off.

By default, it shows changes by anyone in the Channel. To narrow it to your changes only:

1. Hover over the **Recently Edited** header.
2. Click the three-dot menu.
3. Choose **Only me**.

This is especially useful in busy team Channels where everyone else's edits would otherwise crowd out yours.

### The Types section

The **Types** section is the master index of your Channel. It groups every Object by its Type — sub-sections for Notes, Tasks, Books, Pages, every Type that has at least one Object.

Click a Type to open its Type page, which is essentially a built-in Query showing all Objects of that Type. From there you can switch to Grid, Gallery, Board, or any other view.

Inside the Objects section:

#### Quick create

Hover over any Type to reveal a **+** button. Click it to create a new Object of that Type instantly — no menu navigation needed.

#### Reordering Types

Drag a Type's row to reorder. Order is per-member.

#### Hiding empty Types

Only Types that have at least one Object appear here. Create a new Object of a hidden Type, and that Type's section appears automatically. Delete the last Object, and the section disappears.

### Adjusting widget appearance

Every section header has a three-dot menu. Click it to choose how the section's contents are displayed.

For pinned and favorite Objects, you can pick between layouts:

* **Same as Object** — for pinned Queries/Collections, shows them as embedded views
* **Compact** — shows linked sub-Objects nested under each item
* **Detailed** — like Compact but with more details
* **Link** — smallest, just the title and icon

For Queries and Collections, the **Object** layout lets you choose any saved view to embed in the sidebar — so a pinned `Tasks: Today` Query can render as a Board, or a List directly in the sidebar.

<figure><img src="../.gitbook/assets/widget view.png" alt=""><figcaption><p>Widget appearance options</p></figcaption></figure>

### Sidebar display modes: Widgets vs Links

In **Channel Preferences > Sidebar**, you can switch between two overall display modes:

* **Widgets** (default) — rich previews with icons, descriptions, and inline content
* **Links** — a compact list of plain links

**Links** view trades visual richness for density — useful in Channels with hundreds of Objects pinned where the rich previews start to feel heavy. You can switch back to Widgets at any time.

<figure><img src="../.gitbook/assets/sidebar view.png" alt=""><figcaption></figcaption></figure>

### Resizing and collapsing

Drag the right edge of the Sidebar to resize it. You can:

* Make it wider for more space
* Make it narrower to save space
* Collapse it entirely by dragging the edge to the left until it disappears

A collapsed sidebar can be restored by hovering over the left edge of the window — the sidebar pops out temporarily. You can also disable this auto-pop in **Vault Settings > Application > Preferences**.

#### Toggle sidebar shortcut

You can assign a keyboard shortcut to toggle both the **Vault** and **Channel sidebar** at once:

1. Open **Vault Settings > Application > Keyboard Shortcuts**.
2. Find **Toggle Sidebar and Widgets**.
3. Assign a shortcut.

This is useful for quickly switching to focused mode — hide everything to maximize editor space.

### Sidebar in the Compact Vault stripe view

The **Vault** (the panel to the left of the Channel sidebar) has its own compact mode. Drag the Vault's right edge to make it narrower — past a threshold, it switches to **stripe view**:

* Channel and Chat icons only, no labels
* Unread counters still visible
* Mention indicators are hidden (kept only in the regular view)
* Hover over your profile icon to access Help and Gallery
* A **+** button appears at the bottom for creating new Channels

Drag the edge wider to return to the regular Vault layout. See [Manage Sidebar Sections](manage-sidebar-sections.md) for more on sidebar customization.

### Tips

{% hint style="info" %}
**Pin a Query, not just static Objects.** A pinned Query like "Tasks where Status = In Progress" or "Notes where Modified is this week" acts as a live widget — it updates itself as your data changes.
{% endhint %}

{% hint style="info" %}
**Use Tree layout for hierarchical content.** A pinned Project Object using Tree layout shows the project's linked sub-Objects (sub-projects, key documents) inline in the sidebar — like a folder tree.
{% endhint %}

{% hint style="info" %}
**Switch to Links mode for archive Channels.** A Channel where you mostly read rather than create can benefit from the denser Links view — you see more at once.
{% endhint %}
