# Deletion

In Anytype, everything exists as its own independent Object — the same image can be used many times across many documents. Because of this, everything must be intentionally deleted independently. There are no folders you can simply delete with all their contents.

<div data-with-frame="true"><figure><img src="../.gitbook/assets/Docs Deletion System.jpg" alt=""><figcaption></figcaption></figure></div>

## How it works

In Anytype, you must intentionally choose what you want to delete at every moment. Here is a high-level overview of how deletion works in Anytype.

<table><thead><tr><th width="190.3125">Situation</th><th>Traditional</th><th>Anytype</th></tr></thead><tbody><tr><td><strong>Deleting a block</strong></td><td>Pages have a location, so if you delete the block where a page is located, the entire page will be deleted.</td><td>Blocks represent a link to an Object. If you delete a block, the underlying Object still remains.</td></tr><tr><td><strong>Deleting a folder</strong></td><td>Everything inside the folder is deleted with it. This can lead to unintentionally deleting important items deeply hidden in a large folder.</td><td>There are no folders in Anytype. If you delete a <a href="types.md">Type</a>, you will be asked if you want to delete all Objects with it.</td></tr><tr><td><strong>Deleting a database</strong></td><td>Databases contain all of its entries, so if you delete the database, all of the entries go with it.</td><td>Objects are not contained in 'databases' in Anytype (Types, Queries, and Collections). If you delete a 'database', you can preserve all of its entries.</td></tr></tbody></table>

Because Objects in Anytype exist independently from one another, deletion can be more difficult to navigate. The [Cleanup](deletion.md#cleanup) feature helps you ensure your space does not accumulate redundant Objects over time.

## Bin

Deleting an Object will move it to the Bin, otherwise known as 'archiving'. This gives you an opportunity to restore the Object to the space should you change your mind. All Objects stay in the Bin indefinitely until you choose to delete it permanently. You can find the Bin in two locations:

* **Channel Settings** > Preferences > Bin
* **Sidebar** > Manage Sections > Bin

<div data-with-frame="true"><figure><img src="../.gitbook/assets/Docs Bin Intro.jpg" alt=""><figcaption></figcaption></figure></div>

#### Selection

* **Select** — Click on the checkbox to the left of the Object's name.
* **Select All** — Click on the checkbox to the left of the header, next to 'Name'.

Once you have selected at least one Object, you can choose to Delete Permanently or Restore.

#### Permanently Delete

Deleting an Object in your Bin means it will be gone forever and cannot be recovered. You will be asked to confirm you want to proceed every time.

#### Restore

Restoring an Object from your Bin means it will return back to your space. It will retain all of its previous links and settings. This includes restoring Types, Properties, and Templates.

#### Search & Sort

You can search for Objects by their name in the Bin and change the deletion date sorting order. At times, Objects may not have a deletion date so it's best to scroll down the list to find what you're looking for.

## Cleanup

Cleanup shows suggestions for what you could delete to tidy up your space. Objects in this list are **not** in your Bin — they still exist in your space just like any other Object that hasn't been deleted. These are merely suggestions. You can find the Cleanup section alongside the Bin in two locations:

* **Channel Settings** > Preferences > Bin > Cleanup
* **Sidebar** > Manage Sections > Bin > Cleanup

<div data-with-frame="true"><figure><img src="../.gitbook/assets/Docs Bin Cleanup.jpg" alt=""><figcaption></figcaption></figure></div>

### Why it matters

With the way most apps work, users typically expect that deleting something will move it to the bin. Because of the object-based system, this does not always happen in Anytype. This can lead to your space becoming bloated with undeleted files that serve no purpose. Cleanup helps users manage their spaces.

### How does it work?

Imagine you're writing a report. You insert three images into it, then delete one because it doesn't fit the final draft. All three images remain in your space, since every file is an independent Object. But the image you removed from the report is no longer needed; it's just a leftover from your editing process but it still exists in your space. Over time, this clutter builds up, leaving your space full of files that no longer serve a purpose.

Anytype tracks these 'suggested deletions' and lists them in the Cleanup section for you to review. From there, you can dismiss the suggestion or delete the Object permanently. The types of Objects that appear here include:

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
**Use 'delete permanently' cautiously**. It's not possible to recover Objects that have been deleted from your Bin. Only do so if you are certain they are no longer needed.
{% endhint %}

{% hint style="info" %}
**Types, Properties, Templates, etc. can all be found in the Bin**—not just regular documents and files.
{% endhint %}
