---
description: Build precise queries with AND/OR logic and grouped conditions.
---

# Advanced Filters

**Advanced Filters** let you combine multiple filter conditions with AND/OR logic and group them into nested rules — so you can express complex queries like:

> Show me all Tasks where (Priority is High **OR** Due Date is this week) **AND** Status is not Done

Without advanced filters, every condition is joined by AND and applied flatly. Advanced filters give you parentheses — you can express OR, you can group rules, and you can build precise queries that match how you actually think about your data.

## Why it matters

Most filtering needs are simple: "tasks assigned to me", "books I've read". A single condition handles those.

But once your data has any complexity, you start needing things like:

* "Tasks that are urgent **OR** overdue"
* "Notes from this quarter, **but not** the ones tagged 'archive'"
* "Books I've rated 4 or 5 stars **AND** haven't recommended yet"

Each of those needs at least two conditions, and the way they combine matters. Advanced filters make this expressible.

## How to add an Advanced Filter

Advanced filters live alongside basic filters in the filter bar of any Query or Collection.

1. Open a Query or Collection in any list-style view (Grid, List, Gallery, Board).
2. Click the filter icon (or use the **+** button next to the filter bar).
3. Choose **Add advanced filter** in the bottom of the menu.
4. Define your conditions in the dedicated bar that appears.

The basic filter bar shows simple conditions joined by AND. The advanced filter bar shows your full logic — including OR groupings, nested rules, and visual indicators of how conditions combine.

<figure><img src="../../.gitbook/assets/unknown (1).png" alt=""><figcaption></figcaption></figure>

## Building conditions

Each condition has three parts:

* **Property** — which Property to filter by (Status, Priority, Tags, Due Date, etc.)
* **Operator** — how to compare (is, is not, is empty, contains, is greater than, etc.)
* **Value** — what to compare against (a specific value, a list, or a [dynamic value](advanced-filters.md#dynamic-filter-values))

Operators available depend on the Property type:

| Property type             | Operators                                                                                                                                                                             |
| ------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **Text / Title**          | is, is not, contains, doesn't contain, is empty, is not empty                                                                                                                         |
| **Number**                | =, ≠, >, <, ≥, ≤, is empty, is not empty                                                                                                                                              |
| **Date**                  | is, is before, is after, is on or after, is on or before, is within, is empty, is not empty **+** today, tomorrow, yesterday, number of days ago, number of days from now, exact date |
| **Select / Multi-select** | contains any, contains all, doesn't contain, is empty, is not empty                                                                                                                   |
| **Checkbox**              | is checked, is not checked                                                                                                                                                            |
| **Object**                | contains any, contains all, doesn't contain, is empty, is not empty                                                                                                                   |

### Combining with AND / OR

By default, multiple conditions are joined by **AND** — every condition must be true for an Object to match. Switch to **OR** between two conditions and only one of them needs to be true.

To toggle between AND and OR:

1. Click the operator label (AND / OR) between two conditions.
2. The label flips to the other operator.

Visually:

```
Condition A  AND  Condition B  AND  Condition C    → All three must be true
Condition A  OR   Condition B  AND  Condition C    → A is true, OR (B and C are both true)
```

### Grouping conditions

For more complex logic, use **groups** to control precedence — like parentheses in math:

```
(Priority is High  OR  Priority is Urgent)  AND  Status is not Done
```

To create a group:

1. Add the first condition you want to group.
2. Click three-dots next to the values and choose **Turn into group.**
3. Select AND or OR operator.
4. Add next rule.

Grouped conditions are visually indented in the filter bar. You can change the operator inside a group (AND or OR) independently of the operator joining groups.

To delete a rule:

1. Click three-dots next to the values in the group
2. Click **Delete**.

<figure><img src="../../.gitbook/assets/advanced-filters (1).png" alt=""><figcaption></figcaption></figure>

### Dynamic filter values

Filters support **dynamic values** that change based on context:

| Dynamic value    | Where it makes sense                 | Example                             |
| ---------------- | ------------------------------------ | ----------------------------------- |
| **Current User** | Object Property pointing to a Person | Tasks where Assignee = Current User |
| **This Object**  | Inline Queries on Object Properties  | Tasks where Project = This Object   |
| **Today**        | Date Property                        | Notes where Created = Today         |

**Current User** is especially useful for shared Channels — every member sees their own personalized view of a Query without you having to maintain separate Queries per person.

**This Object** works inside [Inline Lists](inline-queries.md) — it scopes the inline Query/Collection to whatever Object is hosting it.&#x20;

### Auto-open value picker

When you select a Property in the filter menu, the value picker now opens automatically — saving you an extra click. Just pick the values you want and the filter is added.

### Active filter bar

Once you have filters configured, they appear in a **dedicated bar above your view**. The Advanced Filters show how many rules are applied to the View.

To edit any active filter, click it. To remove it, click the × on the filter chip. To clear everything in one click, use the **Clear** button at the end of the bar.

### Common filter patterns

#### Tasks I'm working on right now

```
Status is In Progress  AND  Assignee is Current User
```

#### Notes from this week

```
Created is this week
```

#### Books I want to recommend

```
Rating ≥ 4  AND  Recommended-To is empty
```

#### Tasks that are blocked or stale

```
Status is Blocked  OR  (Status is In Progress  AND  Modified is before 7 days ago)
```

#### Items needing review

```
(Type is Document  OR  Type is Note)  AND  Reviewed is unchecked  AND  Created is before this week
```

## Tips

{% hint style="info" %}
**Group OR conditions.** AND has higher default precedence — `A AND B OR C` may not mean what you think. Wrapping the OR in a group makes the intent explicit and unambiguous.
{% endhint %}

{% hint style="info" %}
**Save complex filters as separate Views.** If you've built a filter that's hard to recreate, save it as a View on your Query rather than rebuilding it each time. The Views menu makes them switchable in one click.
{% endhint %}

{% hint style="info" %}
**Use Current User in shared Channel templates.** A "My Tasks" Query in a team Channel works for everyone — each member sees their own tasks. No need to duplicate the Query per person.
{% endhint %}
