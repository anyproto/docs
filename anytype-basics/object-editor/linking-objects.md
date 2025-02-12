---
Description: How to link your Objects with Relations or Simple Links.
---

# Links

### Creating New Links

#### Link to another Object in Anytype

Directly through the canvas by using:

1. **Block Links.** Add the slash character ("/") to invoke a command bar, and then look for the `Link to Object` option in the menu. These can appear either as text or as cards.
2. **Inline Links**. Type @ to invoke the Object picker menu.

With Relations by assigning an Object Relation Type in the Object menu.

#### Link to external Object on your device

If you want to add a link to an external Object on your desktop, please use the links **starting with file:///** plus the local file destination. For example:

* file:///Users/Alex/Downloads/Protocol-Berg.pdf — to open PDFs;
* file:///Users/Alex/Downloads/my\_budget.xlsx — to open spreadsheets (Excel, Numbers).

To add such a link, pick up "Link to website" just like when you add a new link to a website.

#### Date mentions

You can use **Inline Links** to quickly link to either absolute or relative dates.

Some examples:

* @now or @today
* @tomorrow
* @nextweek
* @nextmonth
* @24/8/2023

It's also possible to use `@date` or `/date` to quickly open the date selection menu.

<figure><img src="../../.gitbook/assets/image (3) (1) (1).png" alt="" width="375"><figcaption></figcaption></figure>

#### Link aliases

You can use regular links to link to a specific object in your space using a different name.&#x20;

1. Write the name of your link first.
2. Select the name and press `Ctrl + K`.
3. Search for the object you want to link, and select it.

### Checking Existing Links

#### Relations on the Graph

In your documents you may have multiple references or connections which could be attached to other work in your library. The Graph is the visualizer for this. Objects connected to other Objects, connected to Humans, or Tasks.

Learn more about [relations](../../basics/relations/ "mention") & The [graph.md](../../basics/graph.md "mention") here.

#### Use the Flow

Another option to check which Objects are linked together can be found in the Flow tab next to the Graph.

On the top, center of your screen you will see the option to toggle to **Flow** view. This will show you which Object is linked before and after the current Object you are viewing.

#### Backlinks

We've also recently implemented backlinks as part of our relations system.&#x20;

By default, if the backlinks relation is not empty, you will be able to find it in your featured section. Clicking on it will show a list of all the linked objects.\
If an object has no backlinks, the relation will not be shown in the featured section, but you can still locate it in your object relations panel.

<figure><img src="../../.gitbook/assets/image (2) (1) (1) (1) (1).png" alt=""><figcaption></figcaption></figure>

#### Collections

Collections also use links to manage what is shown in their canvas. To add an existing Object to a Collection, use the **Link To** option from the Object context menu.
