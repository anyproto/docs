# Properties

## What are Properties?

**Properties** are the details you attach to an Object—its due date, status, priority, tags, or any other attribute you care about. Using a spreadsheet analogy, every Object is a row and every Property is a column.&#x20;

<div data-with-frame="true"><figure><img src="../.gitbook/assets/Properties Intro.jpg" alt=""><figcaption></figcaption></figure></div>

## Why it matters

Properties enable you to organize your knowledge into flexible systems. Once your Objects have Properties, you can sort, filter, and query them:&#x20;

* Find all **Tasks** with **Priority** set to **High**,
* Find all **Books** where **Status** is **Reading** and sort by highest **Rating**.&#x20;
* Find all **Ideas** with a **Creation Date** from **Last Year**.&#x20;

### Types vs. Properties

* Think of [Types](types.md) as a group of Properties that all get applied to an Object at the same time.
* Properties exist independently from Types, which means you can use the same property on multiple Types. For example, a Genre Property can be used on both Books and Movies.&#x20;
* A Type can have many Properties attached to it, but they can be hidden from view.&#x20;

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

## Create a Property

Because all [Objects](../creation/objects/) have a [Type](types.md), it's best to create a Property within the context of a Type.&#x20;

#### From the Type View

When viewing a Type, you can click on the 'View settings' button on the top right and select 'Properties'. From this menu, you can also:&#x20;

* Toggle the Properties you want to show on and off. &#x20;
* Rearrange the order of the Properties.
* Remove the Property entirely from the Type.
* Move the Property to the Bin.&#x20;

<div data-with-frame="true"><figure><img src="../.gitbook/assets/Types Create View (1).gif" alt=""><figcaption></figcaption></figure></div>

#### From the Type Edit Menu

[While editing a Type](types.md#editing-types), you can use the 'plus' button of the Properties section to add an existing property or to create a new one.

<div data-with-frame="true"><figure><img src="../.gitbook/assets/Properties Create Type Settings.jpg" alt=""><figcaption></figcaption></figure></div>

#### From Channel Settings

Open your [space](../basics/space/ "mention") settings, and navigate to `Content Model > Properties`. Afterwards, simply click on `New` button to create a new Property.

From here, you can choose a name and a type for your new Property.

<figure><img src="../.gitbook/assets/settings-properties.png" alt=""><figcaption></figcaption></figure>

If you've decided that this Property is no longer relevant, you can use the context menu (mouse right-click) to delete the Property from your Channel.

#### From the Object Editor

You can add a Property to your Objects as you would with any other block in the editor: by using the `+` button or the in-line `/` menu.

<figure><img src="../.gitbook/assets/slashmenu-property.png" alt=""><figcaption></figcaption></figure>

Any Property you create from the object editor will be available for editing in your Channel settings using the steps above.

## Types of Properties <a href="#types-of-relations" id="types-of-relations"></a>

Here are the currently available Property types within Anytype:

* **Text**: accepts free-form text as input.
* **Number**: for all numbers. Different formats are coming soon.
* **Date**: date, with optional time.
* **Select**: categorical property with a predefined list of options. You can choose one.
* **Multi-select**: categorical property with a predefined list of options. You can choose multiple, with no limit.
* **Email/Phone/URL**: special formats for email addresses, phone numbers, or URLs.
* **Checkbox**: a boolean (true/false) value.
* **File & Media**: attach audio, video, or images to view, play, or download.
* **Object**: reference to another object, such as a person, task, or document.

### Managing Properties

You can also manage the Properties for a given Object via **Edit Type** (three-dots menu in the top right corner of any Object).

<figure><img src="../.gitbook/assets/New Type – Default State.png" alt=""><figcaption></figcaption></figure>

The Properties icon lets you view the properties of a specific object, while the Set up menu allows you to manage the properties of its Type – you can add, remove and organize them into different sections:

* **Header** properties appear in the header part of every object of that Type
* **Panel** properties are those that will be shown by pressing Properties icon
