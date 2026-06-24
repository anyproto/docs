# Views

## What are Views?

Views are a visual lens that you place over your content. It allows you to look at the exact same information in different formats, shapes, and orders without ever changing the underlaying content.&#x20;

> **Analogy**: Imagine a building with one hundred people in it. Changing the 'View' doesn't change who is in the building, it just changes where they are. You can have all the people with red clothing in the lobby, while everybody else hides in the basement. Or you can arrange all the people in a long line from shortest to tallest.&#x20;

<div data-with-frame="true"><figure><img src="../.gitbook/assets/Docs Properties Views.gif" alt=""><figcaption></figcaption></figure></div>

## Why it matters

1. With Views, you never need to duplicate content. You can operate from the same set of Objects, just arranged to suit your needs each time.&#x20;
2. With Views, you can surface new perspectives on your content. By using unique combinations of layouts, filters, and sorts, you can organize your information in new ways.&#x20;

## How it works

There are three core components to a View:&#x20;

1. **Layouts** — how Objects are visually structured, such as in a 'gallery layout'.&#x20;
2. **Filters** — which Objects are displayed, such as a filter for 'created this year'.&#x20;
3. **Sorts** — what sequence Objects appear, such as a sort for 'alphabetical'.&#x20;

### Layouts

<table><thead><tr><th width="130.99609375">Options</th><th>Best For</th><th>Extra Options</th></tr></thead><tbody><tr><td><strong>List</strong></td><td>Simple vertical rows</td><td>Compact Mode, Regular Mode</td></tr><tr><td><strong>Grid</strong></td><td>Spreadsheet-like experience</td><td>Wrap Content</td></tr><tr><td><strong>Calendar</strong></td><td>Date and time arrangement</td><td>Date Property</td></tr><tr><td><strong>Kanban</strong></td><td>Grouping and project management</td><td>Group by, Color columns, Cover</td></tr><tr><td><strong>Gallery</strong></td><td>Visual highlights</td><td>Cover, Card Size</td></tr><tr><td><strong>Graph</strong></td><td>Inter-connected relationships</td><td>Graph Settings</td></tr></tbody></table>

{% hint style="warning" %}
Not all views are available on mobile.&#x20;
{% endhint %}

### Filters

Filters narrow the Objects in your View by matching specific conditions. In other words, they hide parts of your data from the View. Each filter has three parts to it:

1. **Property** — which Property to check (such as 'status' or 'due date').&#x20;
2. **Condition** — how to compare (such as 'is not' or 'greater than').&#x20;
3. **Value** — what specific target you're looking for (such as 'in progress' or 'today').&#x20;

Here are some example filters for projects:&#x20;

* To see what's due today: `Due Date` `is` `Today`&#x20;
* To hide completed projects: `Status` `is not` `Done`&#x20;
* To find high-priority items: `Priority` `contains` `Urgent` and `High`

You can apply multiple filters, they are joined by 'AND'. For more advanced filters using 'OR' logic, grouping, and complex conditions, see [Advanced Filters](../advanced/feature-list-by-platform/advanced-filters.md).

### Sorts

Sorts sets the sequence in which your Objects appear in your View. It doesn't hide any data, it just sets the order. Whenever you apply a sort, you have to choose a direction:&#x20;

1. **Ascending** — this will go from lowest to highest ('A to Z' or 'past to future dates').&#x20;
2. **Descending** — this will go from highest to lowest ('Z to A' or 'furthest date first').&#x20;

Here are some common sorts for projects:&#x20;

* To see what's most urgent first: `Due date` sorted by `Ascending`.&#x20;
* To see most recent activity: `Last modified date` sorted by `Ascending`.&#x20;
* To see what's best ranked: `Rating` sroted by `Descending`.&#x20;

You can apply multiple sorts to a View. The first sort will apply, followed by the second, and so forth.&#x20;

## Create & Manage Views

Views are used on all [Types](types.md), [Queries](sets.md), and [Collections](collections.md). By default, every item starts with one pre-set view, but you can add as many custom views as you like. Because views only change how your data is displayed, you can freely edit, delete, or rearrange them without any risk of breaking your underlying information.

#### Creating a View

1. Navigate to any Type, Query, or Collection via the Sidebar.&#x20;
2. Click on the 'plus' button in the View Header, which is below the title area.&#x20;
3. In the 'View settings', you can give it a title, select the layout, and apply filters/sorts.

<div data-with-frame="true"><figure><img src="../.gitbook/assets/Docs Views Create.jpg" alt=""><figcaption></figcaption></figure></div>

#### Change the View settings

Click on the 'View settings' button, which is the icon next to the 'New' button.&#x20;

* **Layout** — change the layout used to visualize the Objects.&#x20;
* **Properties** — change the Properties displayed and add new ones.&#x20;
* **Filter** — apply filters to the View.
* **Sort** — apply sorts to the View.
* **Duplicate view** — create a clone of the View.
* **Remove view** — remove the View (does not affect the Objects).&#x20;

To rearrange the order they appear, click and drag on the View's name that you want to move.&#x20;

<div data-with-frame="true"><figure><img src="../.gitbook/assets/Docs Views Settings.jpg" alt=""><figcaption></figcaption></figure></div>

## Using Views

### Views in Types, Queries, and Collections

Views all follow a three step process: choose a layout, set some filters, and arrange with a sort. Here are some example Views that you could create:&#x20;

* **Gallery layout** filtered with only your **active Projects** sorted by **priority**.&#x20;
* **Calendar layout** with **all your Projects** based on **deadline**.&#x20;
* **Grid layout** filtered for only **Projects assigned to you** sorted by **latest activity**.&#x20;
* **Kanban layout** filtered for **Projects tagged Important** grouped by **current status**.&#x20;

<div><figure><img src="../.gitbook/assets/Docs Views Grid.jpg" alt=""><figcaption><p>Grid Layout</p></figcaption></figure> <figure><img src="../.gitbook/assets/Docs Views List.jpg" alt=""><figcaption><p>List Layout</p></figcaption></figure> <figure><img src="../.gitbook/assets/Docs Views Kanban.jpg" alt=""><figcaption><p>Kanban Layout</p></figcaption></figure> <figure><img src="../.gitbook/assets/Docs Views Gallery.jpg" alt=""><figcaption><p>Gallery Layout</p></figcaption></figure> <figure><img src="../.gitbook/assets/Docs Views Calendar.jpg" alt=""><figcaption><p>Calendar Layout</p></figcaption></figure> <figure><img src="../.gitbook/assets/Docs Views Graph.jpg" alt=""><figcaption><p>Graph Layout</p></figcaption></figure></div>

### Views in Sidebar

You are able to add Views to your Sidebar for immediate access.&#x20;

1. Using the 'three dots' button on the top right corner and select **Pin to Channel**.&#x20;
2. Right click the item in the Sidebar.&#x20;
3. In the menu section 'View', select **Same as Object**.&#x20;
4. If the View is not showing, hover over the icon and click on the dropdown arrow to reveal it.

You can cycle between the various Views you have already setup, right in the Sidebar.&#x20;

<div data-with-frame="true"><figure><img src="../.gitbook/assets/Docs Views Sidebar.gif" alt=""><figcaption></figcaption></figure></div>

### Views in Objects

You can use the Inline Query and Inline Collection blocks in the editor to add Views directly into pages. This enables you to see your Objects right alongside your content.&#x20;

1. While editing a page, open the command menu using the `+` button or `/inline` shortcut:&#x20;
2. Select **Inline Query** to add a [Type](types.md) or [Query](sets.md), and **Inline Collection** for a [Collection](collections.md).&#x20;

<div data-with-frame="true"><figure><img src="../.gitbook/assets/Docs Views Inline.gif" alt=""><figcaption></figcaption></figure></div>

#### Editing Inline Views

Edits made to the View of Inline Queries and Inline Collections is applied only to that block in the Object. That is, editing the Inline View does not affect the 'master View', which is always retained at the [Type](types.md), [Query](sets.md), and [Collection](collections.md) level. This means that you can have multiple versions of the Inline View that's specific to each Object while never affecting the master View.&#x20;

This is not to be mistaken for editing Objects and their Properties, doing so in an Inline View does edit the Object itself and will be reflected across the entire Space.&#x20;

## Bulk editing Objects

You can edit multiple [Objects](../creation/objects/) at the same time—change types, edit properties, and mass delete. This is best done in a View set to the Grid layout, but it also works in other layouts as well.&#x20;

1. Navigate to the View from the Sidebar.&#x20;
2. Select the all Objects you want to edit. You can do this by:
   1. Use the shortcut `Cmd/Ctrl + A` to select all.&#x20;
   2. Click and drag to create a highlight box.&#x20;
   3. Click on the left handle (only in Grid and List layout). `Shift + Click` to add more selections.&#x20;
3. Right-click and choose from various actions: &#x20;
   1. Change Type
   2. Edit Properties
   3. Add to Collection
   4. Export
   5. Duplicate
   6. Move to Bin

<div data-with-frame="true"><figure><img src="../.gitbook/assets/Docs Views Bulk Edit.gif" alt=""><figcaption></figcaption></figure></div>

## Deleting Views

Views are separate from an Object. Deleting a View does not affect the underlying Objects that are part of the View. You can delete them from your Types, Queries, and Collections without worrying about losing your Objects.&#x20;

## Tips

{% hint style="info" %}
**Name your Views by their layout or filter**. By applying useful names, you can more quickly understand what you're navigating such as 'High-priority Tasks' and 'Archived Projects'.
{% endhint %}

{% hint style="info" %}
**When bulk editing Objects, it's best to first setup the View filters** to only show the Objects you want to edit. The makes selection much quicker. You can also create a [Query](sets.md) to do this.&#x20;
{% endhint %}
