---
description: Pre-filled starting points for new Objects.
---

# Templates

A **Template** is a saved layout for a page that you can reuse. Instead of starting every new Note, Task, or Project from a blank page, you define what a good starting point looks like once and it'll form the base for every new Object you create afterwards.

<div data-with-frame="true"><figure><img src="../.gitbook/assets/Docs Template Introduction.jpg" alt=""><figcaption></figcaption></figure></div>

## Why it matters

Templates help you with three things:

* **Standardize your pages** — ensure everything follows the same format.
* **Save time** — set a template once and reuse it forever.
* **Reduce errors** — limit the amount that needs manual entry each time.

## When to use templates

It's best to use templates on Objects that you find yourself repeatedly entering the same content in that follows a similar structure every time. Good examples of this are cooking recipes, book reviews, project dashboards, and content releases.

Conversely, it's best to not put too much into a template that may create a lot of work for you in the future to update. Focus on putting only what truly matters into each template.

## How it works

* Every new Object that's created will use the default Template if it is set.
* Templates are only applied to Objects when they are created. Future updates to a Template will not update Objects created from earlier versions.
* You can have multiple Templates for each [Type](types.md), but only one can be the default.
* You can switch to a different Template when an Object is created, but this option is no longer possible afterwards.
* Templates can also be set for [Queries](queries.md) and [Collections](collections.md).
* Templates can also be set per [View](views.md).

These are all the components you can set with a Template:

<table data-search="false"><thead><tr><th width="181.5">Components</th><th>How can you use it?</th></tr></thead><tbody><tr><td><strong>Title</strong></td><td>'Pre-fill name' will set the same title for every new Object created with this Template. 'Empty-name' will not set any title at all.</td></tr><tr><td><strong>Icon</strong></td><td>Choose an emoticon or upload your own image.</td></tr><tr><td><strong>Cover</strong></td><td>Choose an image from the gallery or upload your own image.</td></tr><tr><td><strong>Description</strong></td><td>Show or hide the description by default with preset text.</td></tr><tr><td><strong>Width</strong></td><td>Change the page width. This can also be set at the Type layout level.</td></tr><tr><td><strong>Properties</strong></td><td>Preset specific values for Properties.</td></tr><tr><td><strong>Blocks</strong></td><td>Preset specific blocks and design layouts for the page.</td></tr></tbody></table>

## Create a Template

Building a Template is exactly the same as building your desired Object. Add all of your desired content blocks, pre-fill your Properties, and give it a name. As you edit the Template, it will auto-save every change you make.

<div data-with-frame="true"><figure><img src="../.gitbook/assets/Docs Templates Setting Up.gif" alt=""><figcaption></figcaption></figure></div>

#### From an existing Object

1. Open the Object you'd like to base a template off of.
2. Click on the 'three dots' button on the top-right corner.
3. Click the menu item **Use as template**.

#### From any Type, Query, or Collection

1. Open the desired Type, Query, or Collection.
2. Click on the 'Templates' button on the right hand side.
3. Click '**+**' to start a new Template.

Setting the default Template here will apply to all Objects created for this Type, Query, or Collection.

#### From the Channel Settings

1. Open **Channel Settings > Content Model > Object Types**.
2. Click the Type you want to add a Template to.
3. Find the **Templates** section in the right panel.
4. Click '**+**' to start a new Template.

#### Editing an existing Template

1. Navigate to the desired Template.
2. While hovering over it, click on the 'three dots' button.
3. Select the menu item **Edit template**.

{% hint style="warning" %}
**Template changes only apply to future Objects that are created with it**. For all Objects already created from past versions of the Template, no updates to the Template will transfer to them. Templates are only applied during Object creation.
{% endhint %}

## Using Templates

#### Create Objects with Templates

1. Create an Object with [your preferred method](../creation/objects/#create-objects).
2. The default Template will be applied automatically.
3. Start editing the Template.

<div data-with-frame="true"><figure><img src="../.gitbook/assets/Docs Template Default.jpg" alt=""><figcaption></figcaption></figure></div>

#### Switching to different Templates

You can have multiple Templates. Before making any edits to your new Object, you have the opportunity to switch from the default Template to a different one.

1. Create a new Object.
2. Click on the button '**This type has # templates**'.
3. Choose your desired Template.

Templates are applied when an Object is created. This is why making an edit to an Object will remove your ability to switch Templates afterwards. An alternative solution is to navigate to the Template and copy + paste the content into your desired Object.

<div data-with-frame="true"><figure><img src="../.gitbook/assets/Docs Templates Switch.gif" alt=""><figcaption></figcaption></figure></div>

#### Change the default Template

1. Navigate to the Type.
2. Click on the 'Templates' button on the right hand side.
3. While hovering over your desired Template, click on the 'three dots' button.
4. Select the menu item **Set as default**.

<div data-with-frame="true"><figure><img src="../.gitbook/assets/Docs Templates Default.jpg" alt=""><figcaption></figcaption></figure></div>

#### Set a Template for a specific View

You can set Templates that are specifically tied to certain [Views](views.md). This means that a Type can have multiple Views and a different Template for each.

1. Navigate to a Type, Query, or Collection.
2. Click on the 'dropdown arrow' next to the 'New' button.
3. Set the **Template for this View**.

While you are in this View, clicking on the 'New' button will automatically apply the Template for this view. This overrides the default Template that is set for the entire Type when you are creating an Object from this View.

<div data-with-frame="true"><figure><img src="../.gitbook/assets/Docs Template View.jpg" alt=""><figcaption></figcaption></figure></div>

#### Locking Templates

If you want to be sure your Template remains consistent, you can lock it to prevent accidental edits. Importantly, locking a Template does not prevent it from being deleted. Deleted Templates can be restored from the Bin. To lock a Template:

1. Edit the Template
2. Click on the 'three dots' button on the top right corner.
3. Select the option **Lock Template**.

<div data-with-frame="true"><figure><img src="../.gitbook/assets/Docs Template Lock.jpg" alt=""><figcaption></figcaption></figure></div>

#### Duplicating Templates

To make a variant of an existing Template:

1. Open the Template.
2. Find the Template you want to copy.
3. Click the three-dot menu > **Duplicate**.
4. Edit the copy to make it your variant.

Useful for incremental refinement or for creating role-specific versions of the same base Template.

#### Template name pre-fill

Templates can include a default name that's pre-filled into new Objects. To control this behavior:

1. Edit the Template.
2. In the title area, you'll see a toggle between **Pre-fill name** and **Empty name**.
   1. **Pre-fill name** — new Objects start with the Template's name (which you can replace by typing)
   2. **Empty name** — new Objects start with a blank title, ready for you to type

Use **Empty name** when the Template's name is just for _finding_ the Template (e.g., "Daily Journal" is the Template name, but you don't want every entry to start with "Daily Journal" as the title).

<div data-with-frame="true"><figure><img src="../.gitbook/assets/Docs Template Title Name.jpg" alt=""><figcaption></figcaption></figure></div>

## Multiple Templates

You can have many Templates for the same Type. Here is some inspiration:

* **Note Type** — Templates for "Daily Journal", "Meeting Note", "Reading Note", "Idea Capture"
* **Task Type** — Templates for "Bug Report", "Feature Request", "Recurring Maintenance"
* **Document Type** — Templates for "Weekly Review", "Tech Spec", "Postmortem", "One-Pager"

## Templates with Properties

Templates can pre-set Property values, making Objects more standardized.

* **Status** = "Draft" by default for new content ideas
* **Priority** = "Low" by default for new Tasks
* **Author** = "Current User" by default for Ideas
* **Tags** = pre-applied tags relevant to the Template

When you create an Object from the Template, these defaults are applied. You can override them on the new Object — the Template's Property values are just starting points.

## Deleting Templates

1. Open the Type's Templates list.
2. Click the three-dot menu next to the Template > **Delete**.

The Template is removed and can be found in the Bin where it can be restored. **Objects created from this Template are not affected** — they keep the content the Template gave them. The Template simply no longer exists for future Object creation.

## Tips

{% hint style="info" %}
**Create your Objects, then create a Template after.** Build the layout you want on a real Object first, iterate until it's right, then save it as a Template. This is more reliable than designing a Template from scratch in the abstract, as it may not truly serve your needs.
{% endhint %}

{% hint style="info" %}
**Set a per-View default for shared Channels.** A team Channel where one View is "Bug Tracker" and another is "Feature Requests" benefits from per-View Templates — Bug Tracker's New button uses the Bug Report Template, Feature Requests uses a different one. Members create the right kind of Object without thinking about it.
{% endhint %}
