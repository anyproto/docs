---
description: A live search of all Objects which share a common Type or Relation
---

# Sets

{% content-ref url="../../use-cases/deep-dive-sets.md" %}
[deep-dive-sets.md](../../use-cases/deep-dive-sets.md)
{% endcontent-ref %}

### Understanding Sets

Lots of people compare Sets with databases, but there's a key difference: Sets don't _store_ Objects like regular databases.

Sets are a way to see a portion of your Graph, and Objects you've created, based on your filtered criteria, and several secondary filters which you can customize. You can think of them as a live filter or query for Objects which share certain criteria - specifically, a Type or a Relation.

#### Sets serve two primary functions:

1. **Organizing and Accessing Objects**\
   \
   We often get requests along the lines of: _How do I find all of the Notes I've created?_\
   \
   One easy way is to create a Set based on Type.\
   For example; Note, which will display every Note you've created in Anytype.\
   \
   If you have specific notes you'd like to frequently access, you can filter them based on Relations you've added to these notes.\
   \
   For instance: Creation Date, Tags, or Priority. (In this sense, Relations behave like attributes).\
   \
   You can then pin your Set to your Favorites menu, where it will sit on your Sidebar, acting like a folder for all Objects that meet certain criteria.
2. **Editing Objects**\
   \
   Sets also provide a way to quickly edit Objects in a list View.\
   \
   You can use multi-select Objects in Sets to delete multiple Objects at once, or to batch update the Object Type. Any Relations added to a Set in the Relation Menu (top right), will be adopted by all new Objects created with the "+ New Object" button.

<figure><img src="../../.gitbook/assets/image (68).png" alt=""><figcaption></figcaption></figure>

### Creating Sets

#### You can create a Set with the + in the bottom-left corner or using the / shortcut menu in the editor.

You'll then need to choose if you want a Set by Type which lets you list all of your Objects of a certain Type, or a Set by Relation which will list all Objects that contain the Relation of your choosing.&#x20;

You can also create a Set by Type from the Object type toggle on a new document.

<figure><img src="../../.gitbook/assets/image (18).png" alt=""><figcaption></figcaption></figure>

#### Next, you need to decide on the purpose of your Set.&#x20;

For example, project management may require Type: Project, for reading list — Book. From the Library, choose an Object Type, click "Create," and choose "Create a set."

This will then create a set of all the Objects with the Type: Books.&#x20;

Now you have an organized selection of all your book objects entered into Anytype.

<figure><img src="../../.gitbook/assets/image (26).png" alt=""><figcaption></figcaption></figure>

### Customizing Your Set

#### Toggle & Add Relations to Objects via Sets

Instead of adding Relations one-by-one to Objects, you can batch-add them to your Set by clicking the filters on the right side.

Here you can toggle on/off any Relations that you would like to see, add another Relation or new relation, and edit the View of the Set here.

![](<../../.gitbook/assets/image (16).png>)

You can add any Relations to be automatically added to your **Objects**, by adding them in the creation process of your **Type**.

See more about how to [create-a-new-type.md](../types/create-a-new-type.md "mention") here. Underneath the title & Template section of the new Type process you'll have the Relation options.

![](<../../.gitbook/assets/image (1) (1) (1) (1) (1) (1).png>)

#### Sorts & Filters

You are also able to sort or filter your set by any relation that you've previously added to the Set.
