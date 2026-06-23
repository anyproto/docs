# Properties

## What are Properties?

**Properties** are the details you attach to an Object—its due date, status, priority, tags, or any other attribute you care about. Using a spreadsheet analogy, think of every Object as a row and every Property as a column.&#x20;

<div data-with-frame="true"><figure><img src="../.gitbook/assets/Properties Intro.jpg" alt=""><figcaption></figcaption></figure></div>

## Why it matters

Properties enable you to organize your knowledge into flexible systems. Once your Objects have Properties, you can sort, filter, and query them:&#x20;

* Find all **Tasks** with **Priority** set to **High**.&#x20;
* Find all **Books** where **Status** is **Reading** and sort by highest **Rating**.&#x20;
* Find all **Ideas** with a **Creation Date** from **Last Year**.&#x20;

## How it works

Properties serve two functions. We'll use a Task Object as an example.&#x20;

**1. Describe Objects** — Add useful and defining details with Properties such as:&#x20;

* Status: In Progress
* Priority: High
* Due Date: Next Friday

**2. Connect Objects** — Link an Object to another through a Property, such as:&#x20;

* Assigned To: → Alex (a Person Object)
* Project: → Website Redesign (a Project Object)

<div data-with-frame="true"><figure><img src="../.gitbook/assets/Properties Example.gif" alt=""><figcaption></figcaption></figure></div>

## What kind of Properties are there <a href="#types-of-relations" id="types-of-relations"></a>

Here are the currently available Property types within Anytype:

<table><thead><tr><th width="189.9609375">Property Type</th><th>Description</th></tr></thead><tbody><tr><td><strong>Text</strong></td><td>Accepts free-form text as input. </td></tr><tr><td><strong>Number</strong></td><td>For all numbers. Different formats are coming soon. </td></tr><tr><td><strong>Date</strong></td><td>Date, with optional time. </td></tr><tr><td><strong>Select</strong></td><td>Predefined list of options. You can choose one. </td></tr><tr><td><strong>Multi-select</strong></td><td>Predefined list of options. You can choose multiple, with no limit. </td></tr><tr><td><strong>Email/Phone/URL</strong></td><td>Special formats for email addresses, phone numbers, or URLs. </td></tr><tr><td><strong>Checkbox</strong></td><td>A true/false value. </td></tr><tr><td><strong>File &#x26; Media</strong></td><td>Attach audio, video, or images to view, play, or download. </td></tr><tr><td><strong>Object</strong></td><td>Reference to another object, such as a person, task, or document. </td></tr></tbody></table>

## Types vs. Properties

* Properties on Objects can exist independently from [Types](types.md). Think of Types as a group of Properties that all get applied to an Object at the same time.
* You can use the same Property on multiple Types. For example, a Genre Property can be used on both Books and Movies.&#x20;
* You can have have a Property on an Object that is not part of its Type. For example, a Favorites Property can be on a Book Object, but not part of the Book Type.&#x20;

## Create & Manage Properties

Because all [Objects](../creation/objects/) have a [Type](types.md), it's best to use Properties within the context of a Type. You can:&#x20;

* Create new Properties.&#x20;
* Add existing Properties.&#x20;
* Rearrange the order.&#x20;
* Toggle visibility.&#x20;
* Remove the Property from the Type.
* Move the Property to the Bin.&#x20;

#### From the Type Edit Menu

[While editing a Type](types.md#editing-types), you can use the 'plus' button of the Properties section to add an existing Property or to create a new one. To edit a Property, simply click on it. The rearrange the order, click and drag on the handle located on the left-hand side.&#x20;

<div data-with-frame="true"><figure><img src="../.gitbook/assets/Properties Create Type Settings.jpg" alt=""><figcaption></figcaption></figure></div>

#### From the Type View

When viewing a Type, you can click on the 'View settings' button on the top right, select **Properties**, and add your desired Property. To edit a Property, simply click on it. The rearrange the order, click and drag on the handle located on the left-hand side.&#x20;

<div data-with-frame="true"><figure><img src="../.gitbook/assets/Types Create View (1).gif" alt=""><figcaption></figcaption></figure></div>

#### From the Object Editor

You can add a Property to your Objects as you would with any other block in the editor: by using the `+` button or the in-line `/` menu.&#x20;

You can add Properties to the Object that are not connected to the Object's Type. However, if you do this often enough, it's best to add the Property to the Object's Type for clearer organization.&#x20;

<div data-with-frame="true"><figure><img src="../.gitbook/assets/Properties Create Command.jpg" alt=""><figcaption></figcaption></figure></div>

#### From Channel Settings

Open your [space-settings.md](../advanced/settings/space-settings.md "mention"), and navigate to Content Model and select **Properties**. Afterwards, simply click on 'New' button to create a new Property.

## Using Properties

Properties are best used in context with their Type. You can manage Properties from the 'Edit Type' panel—[see here](types.md#editing-types).&#x20;

### Properties in Views

Properties are most powerfully used in [views.md](views.md "mention"), which are flexible and customizable ways for you to interact your knowledge. To learn more, please see the [Views](views.md) section.&#x20;

<div data-with-frame="true"><figure><img src="../.gitbook/assets/Docs Properties Views.gif" alt=""><figcaption></figcaption></figure></div>

### Properties in the Object Header

When viewing an Object in a Page format, the Properties can be shown in the Object's Header. This is the section below the title but above the content. There are two layout options:&#x20;

* **Line**—for a more minimal look.&#x20;
* **List**—for displaying more structured information.

These are set on the Type level, which means the layout will be the same for all Objects of that Type.&#x20;

<div data-with-frame="true"><figure><img src="../.gitbook/assets/Properties Header Layouts.jpg" alt=""><figcaption></figcaption></figure></div>

You can use the Object Header to:&#x20;

1. **Show the most relevant Properties**—edit the Type, navigate to the Properties section, drag the Properties you want shown, and arrange the order to your liking. Everything in the 'Properties Panel' and 'Hidden' sections will not display in the Header.&#x20;
2. **Directly edit Properties in the editor**—click on the Property in the Header to make an edit.&#x20;

Properties that are not seen in the Header can still be part of the Type, which are typically used in [Views](views.md).&#x20;

### Properties in Blocks

If you want to have your Properties displayed in the content area of your Pages, you can insert Properties as a block. You can do this with the following methods:&#x20;

* Open the command menu, with the `/` or the 'plus' button, and scroll to the Properties section.
* Type the Property name with the slash command, such as: `/tags` or `/description`.

Property blocks can only be added for Properties that have been added to the Type or already have a value associated with the Property.&#x20;

Once inserted as a block, you can manipulate the Property just like any other block. This is particularly helpful if you want to design nice [Templates](templates.md), as the Object Header is more limited in design flexibility. &#x20;

<div data-with-frame="true"><figure><img src="../.gitbook/assets/Docs Properties Blocks.gif" alt=""><figcaption></figcaption></figure></div>

### Properties Panel

When viewing an Object, you can quickly see all of its Properties by opening the Properties Panel. This is located in the top right corner with the 'information' icon.&#x20;

<div data-with-frame="true"><figure><img src="../.gitbook/assets/Docs Properties Use Panel.jpg" alt=""><figcaption></figcaption></figure></div>

## Tips

{% hint style="info" %}
**Keep it simple, less is more**. When getting started, use as few Properties as possible. Only add new Properties as you find yourself needing more organization power.&#x20;
{% endhint %}

{% hint style="info" %}
**Tags is the easiest way to get started with Properties.** Add relevant tags to all of your documents and create a [Query](sets.md) that groups them all together.&#x20;
{% endhint %}
