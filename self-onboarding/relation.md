# Connect Everything with Relations 🪡

### Understanding Relations

Relations are key to organizing and connecting your Objects and knowledge in Anytype. There are two functions that Relations serve in Anytype:&#x20;

* **Defining attributes:** You can use Relations to define the characteristics of a certain Object. For example, when creating a Task in Anytype, you can add Relations such as _Status_: Done/Not Done, or _Priority_: Low, Medium, or High. If we were to imagine a database, Relations represent the column headers to each row (where column A is the Object). Once you have set your attributes, it becomes possible to sort and filter your Objects according to the Relations you've defined in Set View.

<figure><img src="../.gitbook/assets/Task List.png" alt=""><figcaption></figcaption></figure>

* **Defining connections:** You can also use Relations to link one Object to another. Returning to the example of a Task, you can add the Relation: _Assignee,_ and assign another Object in your Anytype to this task. As above, you can view the Assignees as Relations in Set view, or in Graph view.&#x20;

### Adding & Managing Relations

You can add a Relation to your Objects as you would with any other block in the editor: by using the `+` button or the in-line `/` menu.

You can also manage the Relations for a given Object via its **Relations Panel:** the triangular icon that appears when hovering above the Object name. This Panel shows all relations for that Object.&#x20;

#### Featuring Relations

Here you can add, feature, or modify existing Relations. Featuring Relations allows you to visually prioritize the most relevant Relations for a given Object, as Featured Relations appear directly beneath the Title. You can feature any Relation by clicking ★ next to the relation in the Relations panel.&#x20;

{% embed url="https://vimeo.com/749076155" %}

### Types of Relations

Here are the currently available Relation-types within Anytype:

* **Text**: accepts text as the input.
* **Number**: for all numbers. Different formats are coming soon.
* **Date**: date, optional information for time.
* **Status:** categorical relation wherein you can define a list of options to choose from, like X, Y, or Z.
* **Tag**: another variety of the string with no limits, only one string.
* **Email/phone/URL**: special formats for URL, email, and phone number.
* **Checkbox**: an object with a boolean, string, or link to an object.
* **Media**: audio, movies, or pictures which you can view, play, or download.
* **Object**: reference to a specific object, like a person, task, or document.

{% hint style="warning" %}
At present, you cannot delete relations. So be careful to avoid duplicate relations with the same name.
{% endhint %}
