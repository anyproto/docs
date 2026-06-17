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

## Create a Property

Because all [Objects](../creation/objects/) have a [Type](types.md), it's best to use Properties within the context of a Type. You can create new Properties or add existing Properties to your Types.&#x20;

#### From the Type View

When viewing a Type, you can click on the 'View settings' button on the top right, select **Properties**, and add your desired Property. From this menu, you can also:&#x20;

* Toggle the visibility.
* Rearrange the order.
* Remove the Property from the Type.
* Move the Property to the Bin.&#x20;

<div data-with-frame="true"><figure><img src="../.gitbook/assets/Types Create View (1).gif" alt=""><figcaption></figcaption></figure></div>

#### From the Type Edit Menu

[While editing a Type](types.md#editing-types), you can use the 'plus' button of the Properties section to add an existing property or to create a new one.

<div data-with-frame="true"><figure><img src="../.gitbook/assets/Properties Create Type Settings.jpg" alt=""><figcaption></figcaption></figure></div>

#### From the Object Editor

You can add a Property to your Objects as you would with any other block in the editor: by using the `+` button or the in-line `/` menu.

<div data-with-frame="true"><figure><img src="../.gitbook/assets/Properties Create Command.jpg" alt=""><figcaption></figcaption></figure></div>

#### From Channel Settings

Open your [space-settings.md](../advanced/settings/space-settings.md "mention"), and navigate to `Content Model > Properties`. Afterwards, simply click on `New` button to create a new Property.

## Types of Properties <a href="#types-of-relations" id="types-of-relations"></a>

Here are the currently available Property types within Anytype:

* **Text**: accepts free-form text as input.&#x20;
* **Number**: for all numbers. Different formats are coming soon.&#x20;
* **Date**: date, with optional time.&#x20;
* **Select**: categorical property with a predefined list of options. You can choose one.&#x20;
* **Multi-select**: categorical property with a predefined list of options. You can choose multiple, with no limit.&#x20;
* **Email/Phone/URL**: special formats for email addresses, phone numbers, or URLs.&#x20;
* **Checkbox**: a boolean (true/false) value.&#x20;
* **File & Media**: attach audio, video, or images to view, play, or download.&#x20;
* **Object**: reference to another object, such as a person, task, or document.&#x20;

## Managing Properties

You can also manage the Properties for a given Object via **Edit Type** (three-dots menu in the top right corner of any Object).&#x20;

<figure><img src="../.gitbook/assets/New Type – Default State.png" alt=""><figcaption></figcaption></figure>

The Properties icon lets you view the properties of a specific object, while the Set up menu allows you to manage the properties of its Type – you can add, remove and organize them into different sections:&#x20;

* **Header** properties appear in the header part of every object of that Type
* **Panel** properties are those that will be shown by pressing Properties icon
