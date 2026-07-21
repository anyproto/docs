# Deletion

In Anytype, everything exists as its own independent Object — the same image can be used many times across many documents. Because of this, everything must be intentionally deleted independently as well. You cannot simply delete a folder and all of its contents with a single action.&#x20;

<div data-with-frame="true"><figure><img src="../.gitbook/assets/Docs Deletion System.jpg" alt=""><figcaption></figcaption></figure></div>

## How it works

Here is a high level picture of how deletion works differently in Anytype.&#x20;

<table><thead><tr><th width="190.3125">Situation</th><th>Traditional</th><th>Anytype</th></tr></thead><tbody><tr><td>Deleting a block</td><td>Pages have a location, so if you delete the block where a page is located, the entire page will be deleted. </td><td>Blocks represent a link to an Object. If you delete a block, the underlying Object still remains. </td></tr><tr><td>Deleting a folder</td><td>Everything inside the folder is deleted with it. This can lead to unintentionally deleting important items deeply hidden in a large folder. </td><td>There are no folders in Anytype. If you delete a <a href="types.md">Type</a>, you will be asked if you want to delete all Objects with it. </td></tr><tr><td>Deleting a database</td><td>Databases contain all of its entries, so if you delete the database, all of the entries go with it. </td><td>Objects are not contained in databases in Anytype (Types, Queries, and Collections), you can delete the database while preserving all of the entries. </td></tr></tbody></table>

Because Objects in Anytype exist independently from one another, deletion can be more tricky to navigate. The [Cleanup](deletion.md#cleanup) feature aims to help you ensure your space doesn't have too many redundant Objects in it over time.&#x20;

## Bin

Deleting an Object will move it to the Bin, otherwise known as 'archiving'. This gives you an opportunity to restore the Object to the space should you change your mind. All Objects stay in the Bin indefinitely until you choose to delete it permanently. You can find the Bin in two locations:&#x20;

* **Channel Settings** > Preferences > Bin
* **Sidebar** > Manage Sections > Bin





## Cleanup

Objects listed in this section are suggestions of what could be deleted to clean up your space. Objects in this list are not in your Bin, they exist in your space just like any other Object that has not yet been deleted. They are merely suggestions.  You can find the Cleanup section alongside the Bin in two locations:&#x20;

* **Channel Settings** > Preferences > Bin > Cleanup
* **Sidebar** > Manage Sections > Bin > Cleanup

### Why it matters

With the way most apps work, users typically expect that deleting something will move it to the bin. Because this doesn't always happen on Anytype, it can lead to your space becoming bloated with undeleted files that serve no purpose. Cleanup helps users to manage their spaces.&#x20;

### How does it work?

Imagine you're writing a report. You insert three images into it, then delete one because it doesn't fit the final draft. All three images remain in your space, since every file is an independent Object. But the image you removed from the report is no longer needed; it's just a leftover from your editing process but it still exists in your space. Over time, this kind of clutter builds up, leaving your space full of files that no longer serve a purpose.

Anytype tracks these 'suggested deletions' and lists them in the Cleanup section for you to review. From there, you can dismiss the suggestion or delete the Object permanently. The types of Objects that appear here:

#### Created In

An Object created inside a "parent Object" — and not linked anywhere else — becomes a suggested deletion when that parent Object is deleted. For example:

1. You create Project A.
2. While inside Project A, you use the `/page` command to create an Object called Task X.
3. You delete Project A, leaving Task X orphaned — it's no longer linked to anything.
4. Task X now appears in the Cleanup section as a suggestion.

_Note: If Task X is linked to another Object, such as Project B, it won't appear in Cleanup._

#### Link Removed From

An Object created inside a "parent Object" — and not linked anywhere else — becomes a suggested deletion when its link block is removed from that parent Object. For example:

1. You create a Holiday Plan.
2. Inside Holiday Plan, you drag and drop a PDF of your 30 Aug Flight Ticket.
3. Your flight changes, so you delete the old PDF and add a new one for 1 Sep.
4. The old flight ticket PDF is now orphaned (no other links).
5. Your 30 Aug Flight Ticket appears in the Cleanup section as a suggestion.

_Note: This applies to all other Object types as well, including docs, tasks, images, and videos._

## Tips

{% hint style="info" %}
**Use 'delete permanently' cautiously**. It's not possible to recover any Objects that has been deleted from your Bin. Only do so if you're certain it's no longer needed.&#x20;
{% endhint %}

{% hint style="info" %}
**Types, Properties, Templates, etc. can all be found in the Bin**—not just regular documents and files.&#x20;
{% endhint %}
