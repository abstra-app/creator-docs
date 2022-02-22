---
description: >-
  In this video we will learn how to make queries to the backend that depends of
  some parameter
---

# Creating a simple search using hosted tables

{% embed url="https://youtu.be/wpjJ-kiePTw" %}
This method can be applied for both hosted tables and connectors
{% endembed %}

## Backend

Lets say we have a table with countries like that:

![Table listing countries](<../../.gitbook/assets/image (59).png>)

If we want to make it searchable on you application, we can just create a query with parameter

![We use a parameter called name where we will look as a patter in the middle of the country name](<../../.gitbook/assets/image (65).png>)

Here is the code we are using

```sql
select * from countries where name ilike '%'||$name||'%'
```

## Frontend

In the frontend, we have 2 elements: an text input and a table.

![](<../../.gitbook/assets/image (67) (1).png>)

{% hint style="info" %}
If we want to customize the table, we can use the [collection element](../../docs/front-end/elements/collection.md).
{% endhint %}

Also we need to add a variable which we will use to link the input field and the table query.

![](<../../.gitbook/assets/image (68) (1).png>)

Now we can just link the input field and the variable

![](<../../.gitbook/assets/image (60).png>)

The same with the table linking to the query passing the variable as a parameter

![](<../../.gitbook/assets/image (56).png>)

