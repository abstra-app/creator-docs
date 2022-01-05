---
description: >-
  In this tutorial, you will learn how to make all CRUD operations on one page.
  This is a good pattern for usability because it lowers the friction between
  operations.
---

# Editable list (To Do app)

For this example, we will use our hosted tables feature, but you can use the same techniques with API connectors as well.

## Data model (only for hosted tables)

In this example, we will create a table called `tasks` that will store each task listed (and editable) in our interface.

We will add 2 extra columns (`description` and `done`)

![tasks model](<../../.gitbook/assets/image (59).png>)

Also, we need to add the CRUD operations that will be used by our frontend.

![](<../../.gitbook/assets/image (67).png>)![](<../../.gitbook/assets/image (64) (1).png>)![](<../../.gitbook/assets/image (69) (1).png>)![](<../../.gitbook/assets/image (70).png>)![](<../../.gitbook/assets/image (51).png>)

## Task component

![Task item with a checkbox and an input](<../../.gitbook/assets/image (62) (1) (1).png>)

![Create an task variable for input editing](<../../.gitbook/assets/image (50).png>)

![](<../../.gitbook/assets/image (65) (1).png>)![](<../../.gitbook/assets/image (68).png>)

![Set item on page start](<../../.gitbook/assets/image (52) (1).png>)

![Update task on input change](<../../.gitbook/assets/image (60).png>)

## Main page

![Main page with an collection of task items for each task in List all tasks query](<../../.gitbook/assets/image (58).png>)

![Adding a buttom in the same page for create task](<../../.gitbook/assets/image (66) (1).png>)

![Refresh collection after reload](<../../.gitbook/assets/image (61) (1) (1).png>)

