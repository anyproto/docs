# Properties

Properties are key to organizing and connecting your Objects and knowledge in Anytype. There are two functions that Properties serve in Anytype:

* **Defining attributes:** You can use Properties to define the characteristics of a certain Object.
  * For example, when creating a Task in Anytype, you can add Properties such as _Status_: Done/Not Done, or _Priority_: Low, Medium, or High.
  * If we were to imagine a database, Properties represent the column headers to each row (where column A represents the Object name, and where each row represents an Object).
  * Once you have set your attributes, it becomes possible to sort and filter your Objects according to the Properties you've defined in your Query.
* **Defining connections:** You can also use Properties to link one Object to another.
  * Returning to the example of a Task, you can add the Property: _Linked Projects,_ and connect another Object in your Anytype to this task.
  * As above, you can view the Linked Projects as Properties in a Query, or in your Graph.

<figure><img src="../../.gitbook/assets/image (198).png" alt=""><figcaption></figcaption></figure>

### Create a New Property

#### Creating Properties from the Type Edit Menu

While editing any [Type in your Space settings](./#creating-types-from-space-settings), you can use the `+` button in the top right corner of the Properties section to either add an existing property to the current Type or to create a new one.&#x20;

<div><figure><img src="../../.gitbook/assets/image (123).png" alt=""><figcaption></figcaption></figure> <figure><img src="../../.gitbook/assets/image (124).png" alt=""><figcaption></figcaption></figure></div>

#### Creating Properties from Space Settings

Open your [space.md](../install-and-setup/space.md "mention") settings, and navigate to `Content Model > Properties`. Afterwards, simply click on `New` button to create a new Property.

From here, you can choose a name and a type for your new Property.

<div><figure><img src="../../.gitbook/assets/image (187).png" alt=""><figcaption></figcaption></figure> <figure><img src="../../.gitbook/assets/image (188).png" alt=""><figcaption></figcaption></figure> <figure><img src="../../.gitbook/assets/image (189).png" alt=""><figcaption></figcaption></figure></div>

If you've decided that this Property is no longer relevant, you can use the context menu (mouse right-click) to delete the Property from your space.

<figure><img src="../../.gitbook/assets/image (190).png" alt="" width="375"><figcaption></figcaption></figure>

#### Creating Properties from the Object Editor

You can add a Property to your Objects as you would with any other block in the editor: by using the `+` button or the in-line `/` menu.

<div><figure><img src="../../.gitbook/assets/image (191).png" alt=""><figcaption></figcaption></figure> <figure><img src="../../.gitbook/assets/image (192).png" alt=""><figcaption></figcaption></figure></div>

Any Property you create from the object editor will be available for editing in your space settings using the steps above.

#### Types of Properties <a href="#types-of-relations" id="types-of-relations"></a>

Here are the currently available Property types within Anytype:

* **Text**: accepts text as the input.
* **Number**: for all numbers. Different formats are coming soon.
* **Date**: date, optional information for time.
* **Select:** categorical property wherein you can define a list of options to choose from, like X, Y, or Z.
* **Multi-select**: another variety of the string with no limits, only one string.
* **Email/phone/URL**: special formats for URL, email, and phone number.
* **Checkbox**: an object with a boolean, string, or link to an object.
* **File & Media**: audio, movies, or pictures which you can view, play, or download.
* **Object**: reference to a specific object, like a person, task, or document.

### Managing Properties

You can also manage the Properties for a given Object via its **Properties Panel:** the bullet list icon that appears in the top right corner of the screen. This Panel shows all Properties for that Object.

<div><figure><img src="../../.gitbook/assets/image (125).png" alt=""><figcaption></figcaption></figure> <figure><img src="../../.gitbook/assets/image (126).png" alt=""><figcaption></figcaption></figure></div>

The Properties icon lets you view the properties of a specific object, while the Set up menu allows you to manage the properties of its Type – you can add, remove and organize them into different sections:

* Header properties appear in the header part of every object of that Type
* Panel properties are those that will be shown by pressing Properties icon
* Hidden properties live under the "Hidden" toggle
* Local properties are those that are not associated with the Object's Type

<figure><img src="../../.gitbook/assets/image (127).png" alt="" width="563"><figcaption></figcaption></figure>
