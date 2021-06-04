---
description: Creating a form page and storing data on the interface
---

# Basic form

## Creating a basic form

In the Backend tab. Create the table where the data will be stored.

![](../../.gitbook/assets/1.gif)

Add a `complete` flag where you know if there this form was sent

![](../../.gitbook/assets/2.gif)

Adding the product table

![](../../.gitbook/assets/4.gif)

Adding some mock data for the products table

![](../../.gitbook/assets/5.gif)

Create the product list query

![](../../.gitbook/assets/6.gif)

In the Frontend tab, create a variable to store the form data

![](../../.gitbook/assets/3.gif)

Add the inputs

![](../../.gitbook/assets/7.gif)

Link each input to the variable

![](../../.gitbook/assets/8.gif)

## Creating the order -&gt; product relashionship

Add the relationship column

![](../../.gitbook/assets/adding-relationships-1-.gif)

Create a variable to store the options

![](../../.gitbook/assets/9.gif)

Get the list of products on page start

![](../../.gitbook/assets/10.gif)

Link this list to the dropdown maping the list of product to the [options structure](https://docs.abstra.app/docs/projects/front-end/arguments/argument-types#options)

![](../../.gitbook/assets/11.gif)

Code of mapping:

```javascript
$.products.map(p => ({value: p.id, label: p.name}))
```

To check if is everything alright, test it in the preview mode

![](../../.gitbook/assets/12.gif)

Create the query to insert the data in the database

![](../../.gitbook/assets/13.gif)

Code of query:

```sql
insert into "order"
(email, amount, product_id)
select
email, amount, product_id
from json_populate_record(null::"order", $1)
```

To fininish, let's add the button action

![](../../.gitbook/assets/14.gif)





