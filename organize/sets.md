---
description: Surfacing information from your knowledge base
---

# Queries

Queries are questions you ask your knowledge base that gets saved as a [View](sets.md#views)—a dynamic lens that pulls together [Objects](../creation/objects/) that match your defined criteria. Instead of manually curating a list in your space, you define rules and Anytype will assemble the result automatically and keep it up to date. For example:&#x20;

* Show me everything that's tagged `idea` that was created `in the last 30 days`.&#x20;
* Show me all `projects` where the status is `active`, the priority is `high`, and not marked `done`.&#x20;

<div data-with-frame="true"><figure><img src="../.gitbook/assets/Docs Queries Intro.jpg" alt=""><figcaption></figcaption></figure></div>

## Why it matters

With [Types](types.md) and [Properties](relations.md), your Objects have a lot of structure baked into them—Queries allow you to leverage that structure into useful views.&#x20;

* Surfaces the right things, at the right time, and in the right format.&#x20;
* You don't have to remember where things are.&#x20;
* You don't have to manually organize all your space.&#x20;
* It enables you to handle large amounts of content.&#x20;

## When to use Queries

Use a query when you want to see a slice of your knowledge base that changes over time and would be tedious or error-prone to maintain by hand. You can create and delete Queries without ever affecting the data in your spaces. Here are some examples:&#x20;

* You want a dashboard — a Query for all tasks with a deadline today.
* You have a recurring review — a Query for all notes created this week with no tags.&#x20;
* You want to find something — a Query everything tagged with insight.&#x20;

<div data-with-frame="true"><figure><img src="../.gitbook/assets/Docs Queries Explained.jpg" alt=""><figcaption></figcaption></figure></div>

> **Example**:&#x20;
>
> Say your Space has three Types: Books, Movies, and Games — all sharing a Genre property. You can create a Query filtering for Genre = Science Fiction, and the result is a View showing every science fiction book, movie, and game in your Space, automatically updated as you add new entries.
>
> In other words, the Query is a living answer to: _"What science fiction media do I have?"_ See how to [create this Query below](sets.md#create-a-query).&#x20;

#### Types vs. Queries

[Types](types.md) are effectively built-in Queries, they are inherently the same thing. However, because every Object can only have one Type, Queries really shine when you want to find and group Objects that belong to multiple Types. For example:&#x20;

> You want to find everything science fiction related in your space—create a Query that will pull Objects from the Book, Movie, and Game Types using a 'Science Fiction' Property.&#x20;

#### Collections vs. Queries

When you want a hand-picked list of Objects that have no clear relationships between them, it's best to use a [Collection](collections.md). The issue is that Collections require manual upkeep, so they can quickly become redundant. Queries really shine when you want a group of Objects that say updated. For example:&#x20;

> You want a list of notes that haven't been sorted yet—create a Query that will look for Notes with no category and sorted by most recent date modified. &#x20;

## Create a Query&#x20;

Queries are treated the same as Types, so you can find it in all the same places—in the Sidebar, in the Create Dropdown, and in the Channel Settings. Additionally, all Queries have [Views](views.md) and operate in the same way. To create a Query:&#x20;

1. Create a Query through the [Create menu or Types section](../creation/objects/#how-to-create-objects).&#x20;
2. Choose a **source**. This can be a:
   1. [Type](types.md), such as Tasks, Projects, Books.
   2. [Property](relations.md), such as all Objects with a 'Reviewed' tag property.
3. Set your **filters** and **sorts**.&#x20;
4. Choose a **layout**.

<div data-with-frame="true"><figure><img src="../.gitbook/assets/Docs Queries Create.gif" alt=""><figcaption></figcaption></figure></div>

To learn more about how to manage Queries and their settings, see the [Views](views.md#how-it-works) section.&#x20;

You can also add [Queries to your Sidebar as a Widget](views.md#views-in-sidebar), just like any other View.&#x20;

### Inline Queries&#x20;

You can use the **Inline Query** block in the editor to add a Query directly into pages. This enables you to see your Objects right alongside your content.&#x20;

1. While editing a page, open the command menu using the `+` button or type `/inline query`.
2. Select **Inline Query**.&#x20;
3. Create a new Query or select a pre-existing one.&#x20;

Types are also considered a Query, this is why they also appear in the list of choices.&#x20;

<div data-with-frame="true"><figure><img src="../.gitbook/assets/Docs Query Inline.jpg" alt=""><figcaption></figcaption></figure></div>

### Editing Inline Queries

Edits made to the view of an Inline Query or Inline Collection apply only to that specific block. Editing an Inline View inside an Object does not affect the master View, which is always preserved at the [Type](types.md), [Query](sets.md), or [Collection](collections.md) level. This means each Object can have its own version of the Inline View without ever touching the master.

This is distinct from editing Objects and their Properties on an Inline View—changes made there _do_ affect the Object itself and are reflected across the entire Space.

## Deleting Queries

Just like Views, Queries are separate from the Objects they organize. Deleting a Query does not affect the underlying Objects—you can safely remove them from your space without losing any data.&#x20;

To delete a Query, navigate to your Queries in your Sidebar. You can then delete it like any Object:

* Right-click the Query in the View to reveal a menu, select Move to Bin.&#x20;
* Open it the Query and click on the 'three dots' menu in the top right corner, select Move to Bin.&#x20;

## Tips

{% hint style="info" %}
**Don't create a Query using Types is enough.** You can think of Types as built-in Queries. It's best to create Queries when you're bringing together Objects from multiple different Types.&#x20;
{% endhint %}

{% hint style="info" %}
**Save filter combinations as Views, not new Queries.** If you find yourself filtering the same Query the same way repeatedly, save it as a View. Views let you switch between filter configurations in one click.
{% endhint %}

{% hint style="info" %}
**For manually-curated groupings, use a** [**Collection**](collections.md) **instead.** Queries are rule-driven by the system while Collections are hand-picked by you.
{% endhint %}
