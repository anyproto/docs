---
description: >-
  Does the page become included into another when you create a link or move
  object?
---

# Can pages be nested one to another?

Let's look at an example:

> * I have object A.
> * In object A, I had a link to an existing object B.
> * Then I moved object B inside object A (`move to` action).
> * At this point, I am starting to have a link to object B on object A. What's happened?

Answer: **they both starting to have links to each other**.

We have <mark style="background-color:red;">no nesting</mark> for [object](../fundamentals/object/ "mention"). So object doesn't physically include/store different objects.

All Anytype structures are based on links between objects. Links are directional, so you know that page A links to → page B. You can link oppositely if you need that. You can't use classical hierarchy when files belong to folders and folders create a path. But you can make some of the objects Favourite to be accessible straight from Home.

All objects connections will soon look like an interconnected network:

![Some objects have links from completely different context](<../.gitbook/assets/Screenshot 2021-11-09 at 12.54.59 (1).png>)
