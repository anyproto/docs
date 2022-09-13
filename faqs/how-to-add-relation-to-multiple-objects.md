# How to add relation to multiple objects

### **Using a Type**

Let's look at an example. Say you need to add a new relation, `Color,` to your **Type** `Cat`. And you already have 10 objects of this Type.

1. You need to open [library.md](../features/library.md "mention")
2. Find and open the [Broken link](broken-reference "mention") `Cat`
3. Add a new [relation.md](../self-onboarding/relation.md "mention") `Color` there.

When you open any object `Cat`, you will find `Color` in the relations view and `/` menu.

{% hint style="warning" %}
You cannot edit the default relations in types\*\* created by Anytype\*\*. But you can use [set.md](../self-onboarding/set.md "mention"), which can be used to create a relation in existing objects.
{% endhint %}

### **Using a Set**

Say you need to add `Related` to all your `Tasks`. Unfortunately, you can't change the default relations for this Type.

1. [#create-a-set](../self-onboarding/set.md#create-a-set "mention") with type Task
2. Add a new column. Settings → Relations → \*\*+ \*\*→ `Related`
3. Each object in the Set will now show this relation. Also, see will see at as **suggested** in each object.

![](<../.gitbook/assets/test (1).gif>)
