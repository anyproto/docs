---
title: "Views"
---

Views are visual lenses that you place over your content. They allow you to view the same information in different formats, shapes, and orders without changing the underlying content. [Types](/organize/types/), [Queries](/organize/queries/), and [Collections](/organize/collections/) all use Views to display their content to you.

> **Analogy**: Imagine a building with one hundred people in it. Changing the 'View' doesn't change who is in the building, it just changes where they are. You can have all the people with red clothing in the lobby, while everybody else hides in the basement. Or you can arrange all the people in a long line from shortest to tallest.

![docs properties views](/assets/docs-properties-views.gif)

## Why it matters

1. With Views, you can surface new perspectives on your content, such as time-based items in a calendar or visual-driven content in a gallery. In short, you can arrange and display the same content in multiple different ways.
2. With Views, you never need to duplicate content. You can operate from the same set of Objects, just rearranged to suit your needs each time.

## How it works

There are three core components to a View:

1. **Layouts** — how Objects are visually structured, such as in a 'gallery layout'. [See examples](/organize/views/#views-in-types-queries-and-collections).
2. **Filters** — which Objects are displayed, such as a filter for 'status is complete'.
3. **Sorts** — what sequence Objects appear, such as a sort for 'alphabetical'.

### Layouts

Layouts visually arrange your [Objects](../create/objects/) and their [Properties](/organize/properties/) in ways that make it easier to work with. A series of events on a calendar and a bunch of tasks on a kanban board. Here are some examples of various [layouts in action](/organize/views/#views-in-types-queries-and-collections).

<table><thead><tr><th width="130.99609375">Options</th><th>Best For</th><th>Extra Options</th></tr></thead><tbody><tr><td><strong>List</strong></td><td>Simple vertical rows</td><td>Compact, Regular</td></tr><tr><td><strong>Grid</strong></td><td>Spreadsheet-like experience</td><td>Wrap content</td></tr><tr><td><strong>Calendar</strong></td><td>Date and time arrangement</td><td>Date property</td></tr><tr><td><strong>Kanban</strong></td><td>Grouping and project management</td><td>Group by, Color columns, Cover</td></tr><tr><td><strong>Gallery</strong></td><td>Visual highlights</td><td>Cover, Card size, Icon, Fit media</td></tr><tr><td><strong>Graph</strong></td><td>Inter-connected relationships</td><td>Graph settings</td></tr></tbody></table>

![docs views how layout](/assets/docs-views-how-layout.jpg)

:::caution
Not all views are available on mobile.
:::

### Filters

Filters narrow the Objects in your View by matching specific conditions. In other words, they hide parts of your data from the View. Each filter has three parts to it:

1. **Property** — which Property to check (such as 'status' or 'due date').
2. **Condition** — how to compare (such as 'is not' or 'greater than').
3. **Value** — what specific target you're looking for (such as 'in progress' or 'today').

Here are some example filters for projects:

* To see what's due today: `Due Date` `is` `Today`
* To hide completed projects: `Status` `is not` `Done`
* To find high-priority items: `Priority` `contains` `Urgent` and `High`

You can apply multiple filters, they are joined by 'AND'. For more advanced filters using 'OR' logic, grouping, and complex conditions, see [Advanced Filters](/advanced/feature-list-by-platform/advanced-filters/).

![docs filters](/assets/docs-filters.jpg)

### Sorts

Sorts set the sequence in which your Objects appear in your View. They don't hide any data; they set the order. Whenever you apply a sort, you have to choose a direction:

1. **Ascending** — this will go from lowest to highest ('A to Z' or 'past to future dates').
2. **Descending** — this will go from highest to lowest ('Z to A' or 'furthest date first').

Here are some common sorts for projects:

* To see what's most urgent first: `Due date` sorted by `Ascending`.
* To see most recent activity: `Last modified date` sorted by `Ascending`.
* To see what's best ranked: `Rating` sorted by `Descending`.

You can apply multiple sorts to a View. The first sort will apply, followed by the second, and so forth.

![docs sort](/assets/docs-sort.jpg)

## Create & Manage Views

Views are used on all [Types](/organize/types/), [Queries](/organize/queries/), and [Collections](/organize/collections/). By default, there is one View set, but you can add as many custom Views as you like. Because Views only influence how your data is displayed, you can freely edit, delete, or rearrange them without any risk of affecting your underlying information.

#### Creating a View

1. Navigate to any Type, Query, or Collection via the Sidebar.
2. Click on the 'plus' button in the View Header, which is below the title area.
3. In the 'View settings', you can give it a title, select the layout, and apply filters/sorts.

![docs views create](/assets/docs-views-create.jpg)

#### Change the View settings

Click on the 'View settings' button, which is the icon next to the 'New' button.

* **Layout** — change the layout used to visualize the Objects.
* **Properties** — choose the Properties displayed, its order, and add new ones.
* **Filter & Sort** — apply filters and sorts to the View.
* **Duplicate view** — create a clone of the View with all the same settings.
* **Remove view** — remove the View (does not affect the Objects).

To rearrange the order they appear, click and drag on the View's name that you want to move.

![docs views settings](/assets/docs-views-settings.jpg)

## Using Views

### Views in Types, Queries, and Collections

Views all follow a three step process: choose a layout, set some filters, and arrange with a sort. Here are some example Views that you could create:

* **Gallery layout** filtered with only your **active Projects** sorted by **priority**.
* **Calendar layout** with **all your Projects** based on **deadline**.
* **Grid layout** filtered for only **Projects assigned to you** sorted by **latest activity**.
* **Kanban layout** filtered for **Projects tagged Important** grouped by **current status**.

![Grid Layout](/assets/docs-views-grid.jpg)
_Grid Layout_![List Layout](/assets/docs-views-list.jpg)
_List Layout_![Kanban Layout](/assets/docs-views-kanban.jpg)
_Kanban Layout_![Gallery Layout](/assets/docs-views-gallery.jpg)
_Gallery Layout_![Calendar Layout](/assets/docs-views-calendar.jpg)
_Calendar Layout_![Graph Layout](/assets/docs-views-graph.jpg)
_Graph Layout_

### Views in Sidebar

You are able to add Views to your Sidebar for immediate access, also known as [widgets.md](../basics/sidebar/widgets.md "mention").

1. Using the 'three dots' button on the top right corner and select **Pin to Channel**.
2. Right click the item in the Sidebar.
3. In the menu section 'View', select **Same as Object**.
4. If the View is not showing, hover over the icon and click on the dropdown arrow to reveal it.

You can cycle between the various Views you have already set up, right in the Sidebar.

![docs views sidebar](/assets/docs-views-sidebar.gif)

### Views in Objects

You can use the **Inline Query** and **Inline Collection** blocks in the editor to add Views directly into pages. This enables you to see your Objects right alongside your content.

1. While editing a page, open the command menu using the `+` button or `/inline` shortcut:
2. Select **Inline Query** to add a [Type](/organize/types/) or [Query](/organize/queries/), and **Inline Collection** for a [Collection](/organize/collections/).

Edits made to the view of an Inline Query or Inline Collection apply only to that specific block. Editing an Inline View inside an Object does not affect the master View, which is always preserved at the [Type](/organize/types/), [Query](/organize/queries/), or [Collection](/organize/collections/) level. This means each Object can have its own version of the Inline View without ever touching the master.

This is distinct from editing Objects and their Properties on an Inline View—changes made there _do_ affect the Object itself and are reflected across the entire Space.

![docs views inline](/assets/docs-views-inline.gif)

### Search in Views

In the View toolbar next to the 'New' button, there is a search icon. Using search here filters the Objects in the View based on the text you enter. This is great for temporarily narrowing down your Objects even further.

![docs views search](/assets/docs-views-search.jpg)

### Bulk editing Objects

You can edit multiple [Objects](../create/objects/) at the same time—change types, edit properties, and mass delete. This is best done in a View set to the Grid layout, but it also works in other layouts as well.

1. Navigate to the View from the Sidebar.
2. Select all Objects you want to edit. You can do this by:
   1. Use the shortcut `Cmd/Ctrl + A` to select all.
   2. Click and drag to create a highlight box.
   3. Click on the left handle (only in Grid and List layout). `Shift + Click` to add more selections.
3. Right-click and choose from various actions:
   1. Change Type
   2. Edit Properties
   3. Add to Collection
   4. Export
   5. Duplicate
   6. Move to Bin

![docs views bulk edit](/assets/docs-views-bulk-edit.gif)

### Dragging Objects between Views

When you drag and drop an Object from one View to another, its Properties update to match that View's filters automatically. For example: drag a task from your 'All' View to your 'Completed' View, and the Status Property updates to "Done."

![docs views drag](/assets/docs-views-drag.gif)

## Deleting Views

Views are separate from the Objects they organize. Deleting a View does not affect the underlying Objects — you can safely remove a View from a Type, Query, or Collection without losing any data.

To delete a View, right-click it to reveal a menu. Alternatively, you can delete it from the View settings in the View toolbar.

## Tips

:::note
**Name your Views by their layout or filter**. By applying useful names, you can more quickly understand what you're navigating such as 'High-priority Tasks' and 'Archived Projects'.
:::

:::note
**When bulk editing Objects, it's best to first set up the View filters** to show only the Objects you want to edit. This makes selection much quicker. You can also create a [Query](/organize/queries/) to do this.
:::
