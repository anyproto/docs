---
Description: How to link your Objects together.
description: Creating relationships in your knowledge base
---

# Links

Linking on Anytype is what turns a bunch of separate notes into a connected knowledge base. When you link a 'Task Object' to a 'Project Object', you are saying that these are related. This relationship is registered in Anytype as a link and becomes visible in your Knowledge Graph—which is a mind map of your entire space.

Over time, these connections become incredibly valuable. You can trace how ideas relate, see what's connected to a project, or discover patterns you didn't plan for.

<div data-with-frame="true"><figure><img src="../.gitbook/assets/Docs Links Intro Graph.gif" alt=""><figcaption></figcaption></figure></div>

## How to link

Anytype offers multiple ways to create links, each useful in different situations:

| Method             | What it does                                 | Best for                             |
| ------------------ | -------------------------------------------- | ------------------------------------ |
| **Block Links**    | Adds a visible card or text link on the Page | Prominent references you want to see |
| **Property Links** | Adds a property to an Object.                | Subtle references used to organize   |
| **Date Links**     | Adds a date reference to an Object           | Time references used for chronology  |

## Creating links

### Link to an Object

Directly through the editor by using:

1. **Block Links** — Type `/link`. These appear as cards.
2. **Inline Links** — Type `@` and the object name. These appear as rich text.
3. **Link Alias** — Highlight text, `Cmd/Ctrl + Shift + K`, select the link. These appear as hyperlinked text, good for alternative names.

<div data-with-frame="true"><figure><img src="../.gitbook/assets/Docs Linking Objects.jpg" alt=""><figcaption></figcaption></figure></div>

### Link to a Property

When viewing an Object, you can add links to [properties.md](../organize/properties.md "mention") using:

1. [**Object Header**](../organize/properties.md#properties-in-the-object-header) — Select a property from the header. If the property is not visible, add it to the header from the [type settings](../organize/properties.md#create-and-manage-properties).
2. [**Block Menu**](editor/#adding-blocks) — Add an inline property block from the menu using the plus button or slash command.

Alternatively, you can add a property from [views.md](../organize/views.md "mention"). This is better when you are editing properties of multiple Objects.

<div data-with-frame="true"><figure><img src="../.gitbook/assets/Docs Links Properties.gif" alt=""><figcaption></figcaption></figure></div>

### Link to a Date

You can link to a specific date by typing the `@date` shortcut in the editor. Alternatively, you can type `@today`, `@tomorrow`, or `@specific date`. You can also click into a specific date block to reveal objects related to that date.

<div data-with-frame="true"><figure><img src="../.gitbook/assets/Docs Links Date.jpg" alt=""><figcaption></figcaption></figure></div>

<div data-with-frame="true"><figure><img src="../.gitbook/assets/Doc Link Date.gif" alt=""><figcaption></figcaption></figure></div>

### Link to external files

If you want to add a link to an external Object on your desktop, use links starting with **file:///** followed by the local file path. For example:

* `file:///Users/Name/Downloads/Protocol-Berg.pdf` — to open PDFs;
* `file:///Users/Name/Downloads/my_budget.xlsx` — to open spreadsheets (Excel, Numbers).

To add such a link, select the "Link to website" in the editor just like when you add a new link to a website.

## Viewing Links

#### Backlinks

You can use the Backlinks property in the Object Header to check which Objects link to the currently opened one. If you cannot locate the Backlinks property, go to the Type settings and add it to Header section. [See here for more details](../organize/properties.md#create-and-manage-properties).

<div data-with-frame="true"><figure><img src="../.gitbook/assets/Docs Link Back.gif" alt=""><figcaption></figcaption></figure></div>

#### Knowledge Graph

In your documents you may have multiple connections which could be attached to other objects in your space. The Graph is the best visualizer for this, showing the complete web of connections for all objects. Click on the graph icon on the top left of the editor to access the Graph.

<div data-with-frame="true"><figure><img src="../.gitbook/assets/Docs Links Backlink Graph.gif" alt=""><figcaption></figcaption></figure></div>

Learn more about [properties.md](../organize/properties.md "mention") and the [graph.md](../advanced/feature-list-by-platform/graph.md "mention") with these links.
