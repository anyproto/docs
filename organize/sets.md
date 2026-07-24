---
description: Surfacing information from your knowledge base
---

# Queries

A Query is a question you ask your knowledge base—answered instantly and kept up to date automatically. Rather than manually curating a list of things you're looking for, you define the criteria and the Query assembles the result for you as a [View](views.md). For example:

* Show me everything that's tagged `idea` that was created `in the last 30 days`.
* Show me all my work where the status is `active`, the priority is `high`, and not marked as `done`.

<div data-with-frame="true"><figure><img src="../.gitbook/assets/Docs Queries Intro.jpg" alt=""><figcaption></figcaption></figure></div>

## Why it matters

[Types](types.md) and [Properties](relations.md) give your Objects structure, Queries then go and turn that structure into useful answers.

* Instead of remembering where things are, the right Objects get surfaced at the right time, in the right format.
* Instead of manually organizing everything, you define rules once and Queries keep up with your content as it grows.

## When to use Queries

Use a query when you want to see a slice of your knowledge base that changes over time and would be tedious to maintain by hand. You can create and delete Queries without ever affecting the data in your spaces. Here are some examples:

* You want a dashboard — a Query for everything that has a deadline set for `today`.
* You have a recurring review — a Query for everything with a `triage` status sorted by oldest first.
* You want to find something — a Query for everything tagged with `insight`.

<div data-with-frame="true"><figure><img src="../.gitbook/assets/Docs Queries Explained.jpg" alt=""><figcaption></figcaption></figure></div>

> **Example**:
>
> Say your Space has three Types: Books, Movies, and Games — all sharing a Genre property. You can create a Query filtering for Genre = Science Fiction, and the result is a View showing every science fiction book, movie, and game in your Space, automatically updated as you add new entries.
>
> In other words, the Query is a living answer to: _"What science fiction media do I have?"_ See how to [create this Query below](sets.md#create-a-query).

#### Types vs. Queries

[Types](types.md) are effectively built-in Queries, they are the same thing. However, because every Object can only have one Type, Queries really shine when you want to find and group Objects that belong to multiple Types.

> **Example**:
>
> You want to find everything related to privacy in your space. You create a Query that looks for all Objects tagged with 'privacy'. This may pull Objects from various Types, such as Projects, Tasks, Bookmarks, Notes, Films, and News Articles.

#### Collections vs. Queries

Use a [Collection](collections.md) when you want a hand-picked group of Objects with no clear relationship between them. The tradeoff is manual upkeep — Collections don't update themselves, so they can fall out of date as your Space grows. Queries shine when the group has a logical rule behind it. If you can define it as criteria, let Anytype maintain it for you.

> **Example**:
>
> You want to see everything in your Space that hasn't been sorted yet. Create a Query filtering for Objects with no tags, sorted by date modified. This way, you'll always have an up-to-date inbox of unorganized content to sort through, no matter how much your Space evolves.

## Create a Query

Queries live in all the same places as Types—the Sidebar, the Create menu, and Channel Settings. And like Types, every Query has Views that work the same way. To create a Query:

1. In the Sidebar, click on the [Create Dropdown button](../creation/objects/#create-menu) and select **Query**.
2. Choose a **source**. This can be a:
   1. [Type](types.md), such as Tasks, Projects, Books.
   2. [Property](relations.md), such as all Objects with a 'Reviewed' tag property.
3. Set your **filters** and **sorts**.
4. Choose a **layout**.

<div data-with-frame="true"><figure><img src="../.gitbook/assets/Docs Queries Create.jpg" alt=""><figcaption></figcaption></figure></div>

<div data-with-frame="true"><figure><img src="../.gitbook/assets/Docs Queries Create.gif" alt=""><figcaption></figcaption></figure></div>

## Using Queries

To learn more about how to manage Queries and their settings, see the [Views](views.md#how-it-works) section.

### Sidebar Widget

You can also add [Queries to your Sidebar as a Widget](views.md#views-in-sidebar), just like any other View.

### Inline Queries

You can use the **Inline Query** block in the editor to add a Query directly into pages. This enables you to see your Objects right alongside your content.

1. While editing a page, open the command menu using the `+` button or type `/inline query`.
2. Select **Inline Query**.
3. Create a new Query or select a pre-existing one.

Types are also considered a Query, this is why they also appear in the list of choices.

<div data-with-frame="true"><figure><img src="../.gitbook/assets/Docs Query Inline.jpg" alt=""><figcaption></figcaption></figure></div>

#### Editing Inline Queries

Edits made to the View of an Inline Query apply only to that specific block. Editing an Inline View inside an Object doesn't affect the master View — that stays intact at the [Type](types.md), [Query](sets.md), or [Collection](collections.md) level. This means each Object can have its own version of the Inline View without ever touching the master.

This is different from editing actual Objects and their Properties through an Inline View: those changes **do** affect the underlying Objects and are reflected everywhere they appear across the Space.

## Deleting Queries

Just like Views, Queries are separate from the Objects they organize. Deleting a Query does not affect the underlying Objects—you can safely remove them from your space without losing any data.

To delete a Query, navigate to your Queries in your Sidebar. You can then delete it like any Object:

* Right-click the Query in the View to reveal a menu, select Move to Bin.
* Open the Query and click on the 'three dots' menu in the top right corner, select Move to Bin.

## Tips

{% hint style="info" %}
**Don't create a Query when a Type is enough.** You can think of Types as built-in Queries. It's best to create Queries when you're bringing together Objects from multiple different Types.
{% endhint %}

{% hint style="info" %}
**Save filter combinations as Views, not new Queries.** If you find yourself filtering the same Query the same way repeatedly, save it as a View. Views let you switch between filter configurations in one click.
{% endhint %}

{% hint style="info" %}
**For manually-curated groupings, use a** [**Collection**](collections.md) **instead.** Queries are rule-driven by the system while Collections are hand-picked by you.
{% endhint %}
