# Replicating an ER Diagram on Hosted Tables

In this tutorial we will show you how to create a database with foreign-key relationships with hosted tables based on the following ER diagram.

![](../../.gitbook/assets/er.png)

### Creating the tables

Creating tables with Abstra is easy. Just go to **Backend** &gt; **Hosted Tables** and click on the add button. By default we create the columns **id** \(int\), **created\_at** \(timestamp without timezone\) and **updated\_at** \(timestamp without timezone\). This columns don't need to be filled when inserting or updating the database, they are automatically filled. After that you can create the columns for you table:

**Customers** \(**customer\_name** _varchar_ NOT NULL\)

![](../../.gitbook/assets/customers.gif)

**Orders** \(**order\_date** _date_ NOT NULL\)

![](../../.gitbook/assets/order.gif)

**Shipments** \(**shipment\_date** _date_ NOT NULL\)

![](../../.gitbook/assets/shipments.gif)

After you finish you can see the diagram of your database:

### Creating the relations

In the ER diagram we have two relations:

* customer\_id in Orders points to Customers
* order\_is in Shipments points to Orders  

With Abstra creating relations is as easy as creating another column: select the date type **reference**, select the **table** and then the **column**.

**Orders** \(**customer\_id** _int_ NOT NULL\)

![](../../.gitbook/assets/customer_id.gif)

**Shipments** \(**order\_id** _int_ NOT NULL\)

![](../../.gitbook/assets/order_id.gif)

You are done! Now you can see the diagram of your database and check for the relations:

![](../../.gitbook/assets/diagram-viw.gif)

