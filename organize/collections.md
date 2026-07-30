---
description: Hand-curated groupings of Objects.
---

# Collections

A Collection is a container of hand-picked Objects—the closest thing to a folder in Anytype. You decide what goes in, and Objects stay in the Collection until you remove them. Importantly, Objects exist independently of Collections. The same Object can live in multiple Collections at once, and removing an Object from a Collection doesn't delete it — it simply stops being part of that Collection.

<div data-with-frame="true"><figure><img src="../.gitbook/assets/Docs Collections Intro.jpg" alt=""><figcaption></figcaption></figure></div>

## Why it matters

When there's a clear relationship, it's easy to bring Objects together using a [Query](queries.md), such as 'everything tagged inspiration'. But when there isn't a clear [Property](properties.md) or [Type](types.md) that can link everything together, this is when Collections work best. It's a curated container for everything you see having a relationship together but the system can't easily define.

## When to use Collections

The easiest way to understand Collections is to compare them with [Queries](queries.md). With Collections, you're curating a group of Objects that don't change much over time. With Queries, you're filtering Objects that likely change over time.

Think of a Collection as something you curate by hand—like 'Grandma's Favorites.' Think of a Query as something you define with rules and filters—like everything tagged with 'important.'

| Query                                     | Collection                                                                                 |
| ----------------------------------------- | ------------------------------------------------------------------------------------------ |
| All your media with a rating '4 or above' | Everything you want to do on holiday: books to read, tasks to complete, locations to visit |
| Everything marked as 'high priority'      | Onboarding materials to share with a colleague: dashboards, people, docs                   |
| Everything tagged with 'family'           | Resources that help with a project: YouTube video, PDFs, and notes                         |

**Collections shine with Objects that are loosely connected.** For example, a Collection titled "Q1 Marketing" might hold tasks, design files, news articles, organizations, and meeting notes. Using a Collection can keep these Objects together without forcing them into a single Type or requiring shared Properties for a Query to find them.

**Queries shine when you want a group of Objects to update automatically over time.** For example, a Query for "everything with an end date set for today" will automatically surface matching tasks, projects, and events to you as dates change. There's no manual curation required.

## Create a Collection

Collections live in all the same places as [Types](types.md)—the Sidebar, the Create menu, and Channel Settings. And like Types, every Collection has Views that work in the same way.

To create a Collection:

1. In the Sidebar, click on the [Create Dropdown button](../create/objects/#create-menu) and select **Collection**.
2. Add existing Objects from your space or create new ones.
3. Set your **filters** and **sorts**.
4. Choose a **layout**.

<div data-with-frame="true"><figure><img src="../.gitbook/assets/Docs Collections Create.jpg" alt=""><figcaption></figcaption></figure></div>

<div data-with-frame="true"><figure><img src="../.gitbook/assets/Docs Collections Create Add.gif" alt=""><figcaption></figcaption></figure></div>

## Using Collections

To learn more about how to manage Collections and their settings, see the [Views](views.md#how-it-works) section.

### Add & remove Objects

You can add an Object to as many Collections as you like—this will create a link between them. Objects remain in the Collections you add them to until you remove them.

#### **To add an Object**

* Right click the Object in a [View](views.md) or open the 'three dots' menu in the top right corner.
* From the menu, select **Add to Collection**, and choose from the list of options available.

<div data-with-frame="true"><figure><img src="../.gitbook/assets/Docs Collections Add.jpg" alt=""><figcaption></figcaption></figure></div>

#### **To remove an Object**

1. Navigate to the Collection from the Sidebar.
2. Right click the Object, and select:
   1. **Unlink from Collection** — removes it from the Collection but keeps the Object in the space.
   2. **Move to Bin** — deletes the Object from all Collections and the entire space, but it can be restored from the Bin.

<div data-with-frame="true"><figure><img src="../.gitbook/assets/Docs Collections Unlink.jpg" alt=""><figcaption></figcaption></figure></div>

#### **To edit in bulk**

Use the [bulk-editing feature in Views](views.md#bulk-editing-objects) to organize many Objects at the same time in a Collection. You can create a Query to find the Objects you're looking for, and then add them all to a Collection in bulk.

#### To set a default Type

When adding a new Object into a Collection, you can choose the default [Type](types.md) and [Template](templates.md) used. When viewing a Collection, click on the dropdown button next to 'New' to change the default.

### Inline Collections

You can use the **Inline Collection** block in the editor to add a Collection directly into pages. This enables you to see your Objects right alongside your content.

1. While editing a page, open the command menu using the `+` button or type `/inline collection`.
2. Select **Inline Collection**.
3. Create a new Collection or select a pre-existing one.

<div data-with-frame="true"><figure><img src="../.gitbook/assets/Docs Collections Inline.jpg" alt=""><figcaption></figcaption></figure></div>

#### Editing Inline Collections

Edits made to the View of an Inline Collection apply only to that specific block. Editing an Inline View inside an Object doesn't affect the master View — that stays intact at the [Type](types.md), [Query](queries.md), or [Collection](collections.md) level. This means each Object can have its own version of the Inline View without ever touching the master.

This is different from editing actual Objects and their Properties through an Inline View: those changes **do** affect the underlying Objects and are reflected everywhere they appear across the Space.

### Folder-like Widget

You can add [Collections to your Sidebar as a Widget](views.md#views-in-sidebar), just like any other View. However, instead of using Collections to simulate a [hierarchical folder-like structure in your Sidebar](../basics/sidebar/widgets.md#layout-options), you can create a Page with link blocks:

1. Create any Object with a Page format.
2. In the editor, add links to your desired Objects using the `/link` or `@` blocks. This can be to regular Objects, Types, Queries, or Collections.
3. Arrange the blocks on the Page to represent your hierarchy.
4. Pin the Object to the Sidebar.
5. Right-click the Widget and select 'Hierarchical Structure' in the view setting.
6. To expand each layer, click on the dropdown arrow near the icon.

<div data-with-frame="true"><figure><img src="../.gitbook/assets/Docs Collections Widget Folder-like.jpg" alt=""><figcaption></figcaption></figure></div>

### Uploading files from desktop

You can drag and drop a folder from your desktop into a Collection in Anytype. This will upload all the files in the folder and package them into a single Collection. This is a great way to bring an existing on-disk archive (a photo collection, a project folder, a music library) into your space.

1. Select and drag a folder from your desktop.
2. Drop the folder onto an open Collection.

<div data-with-frame="true"><figure><img src="../.gitbook/assets/Docs Collections Drag Folder.gif" alt=""><figcaption></figcaption></figure></div>

## Deleting Collections

Just like Views, Collections are separate from the Objects they organize. Deleting a Collection does not affect the underlying Objects—you can safely remove them from your space without losing any data. To delete a Collection, navigate to your Collection in your Sidebar. You can then delete it like any Object:

* Right-click the Collection to reveal a menu, select Move to Bin.
* Open the Collection and click on the 'three dots' menu in the top right corner, select Move to Bin.

## Tips

{% hint style="info" %}
**Collections are a quick and dirty way to get organized.** While Queries are best for staying organized in the long run, Collections require less thinking and planning. Create as many as you like, as deleting them has no impact on the Objects they contain.
{% endhint %}

{% hint style="info" %}
**Pin project Collections to your sidebar.** A pinned project Collection acts as a project hub — one click to see everything in scope.
{% endhint %}
