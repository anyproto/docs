# Properties

## What are Properties?

**Properties** are the details you attach to an Object—its due date, status, priority, tags, or any other attribute you care about. Using a spreadsheet analogy, every Object is a row and every Property is a column.&#x20;

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

## Types of Properties <a href="#types-of-relations" id="types-of-relations"></a>

Here are the currently available Property types within Anytype:

<table><thead><tr><th width="189.9609375">Property Type</th><th>Description</th></tr></thead><tbody><tr><td><strong>Text</strong></td><td>Accepts free-form text as input. </td></tr><tr><td><strong>Number</strong></td><td>For all numbers. Different formats are coming soon. </td></tr><tr><td><strong>Date</strong></td><td>Date, with optional time. </td></tr><tr><td><strong>Select</strong></td><td>Predefined list of options. You can choose one. </td></tr><tr><td><strong>Multi-select</strong></td><td>Predefined list of options. You can choose multiple, with no limit. </td></tr><tr><td><strong>Email/Phone/URL</strong></td><td>Special formats for email addresses, phone numbers, or URLs. </td></tr><tr><td><strong>Checkbox</strong></td><td>A true/false value. </td></tr><tr><td><strong>File &#x26; Media</strong></td><td>Attach audio, video, or images to view, play, or download. </td></tr><tr><td><strong>Object</strong></td><td>Reference to another object, such as a person, task, or document. </td></tr></tbody></table>

## Using Properties

Although Objects can have Properties independent from their Type, it's best to use them in the context of their Type. You can manage Properties from the Edit Type panel—[see here](types.md#editing-types).&#x20;

### Properties in the Object Header

When viewing an Object in a Page format, the Properties can be shown in the Object's Header. This is the section below the title but above the content. There are two layout options that are set on the Type level—it will be the same for all Objects of that Type.&#x20;

* **Line**—for a more minimal look.&#x20;
* **List**—for displaying more structured information.

<div data-with-frame="true"><figure><img src="../.gitbook/assets/Properties Header Layouts.jpg" alt=""><figcaption></figcaption></figure></div>

You can use the Object Header to:&#x20;

1. **Show the most relevant Properties**—edit the Type, navigate to the Properties section, drag the Properties you want shown, and arrange the order to your liking. &#x20;
2. **Directly edit Properties in the editor**—click on the Property in the Header to make an edit.&#x20;

Properties that are not seen in the Header can still be part of the Type, which are typically used in [Views](views.md).&#x20;

### Properties in Views

Properties are most powerfully used in [views.md](views.md "mention"), which are flexible and customizable ways for you to interact your knowledge. Tasks sorted by priority on a board, upcoming events in a calendar, and recipes in a labelled list. To learn more, please see [Views](views.md) section.&#x20;







### Properties in Blocks





### Properties Panel







You can also manage the Properties for a given Object via **Edit Type** (three-dots menu in the top right corner of any Object).&#x20;

#### From editing Type



#### From editing View



<figure><img src="../.gitbook/assets/New Type – Default State.png" alt=""><figcaption></figcaption></figure>

The Properties icon lets you view the properties of a specific object, while the Set up menu allows you to manage the properties of its Type – you can add, remove and organize them into different sections:&#x20;

* **Header** properties appear in the header part of every object of that Type
* **Panel** properties are those that will be shown by pressing Properties icon
