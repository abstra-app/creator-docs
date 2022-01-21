---
description: You don't have to manage a database to have your data organized.
---

# Google Sheets

This connector is used to access your google spreadsheets with Abstra. Create the connector and select the spreadsheet in order to begin using it.

You need to authorize access to the specific spreadsheets you need

![](<../../../.gitbook/assets/image (36).png>)

Select the spreadsheet

![](<../../../.gitbook/assets/image (31).png>)

These are the methods you can use to interact with your spreadsheet:

* Get range
* Insert Row
* Update Rows
* Delete Rows

#### Get Range

With this method, you can select a range from the spreadsheet using the A1 notation

![](<../../../.gitbook/assets/image (62).png>)

If you choose to use the first row as a header, the return will be an array of JSON objects, with the keys being the first row of the range, otherwise, the return will be an array of arrays, each one representing a row on the table.

![Examples of the value the method returns, with and without selecting to use the first row as header](<../../../.gitbook/assets/image (54) (1).png>)

#### Insert Row

With this method, you can insert a row in a table that is in your spreadsheet. You just need to fill the range of the table you are inserting the values, and they will be added to the first empty row in that range or bellow it. If you select the _Use first row as header_ option, the value can be a JSON object with the keys being the names of the columns, otherwise, the value has to be an array representing the row.

![Examples for the insert row value, with and without using the first row as header](<../../../.gitbook/assets/image (61).png>)

#### Update Rows

With this method, you can update rows in a table that is in your spreadsheet. You just need to fill the range of the table you are updating the values, fill the filter and the new values for the rows that match the filter. If you select the _Use first row as header_ option, the filter and value can be a JSON object with the keys being the names of the columns, otherwise, they should be JSON objects where the keys are the indexes of the columns in their order. Only the values you add to the update are going to be changed in the matched rows.

![Examples for updating all items where id equals 3, setting their value to R$5,00](<../../../.gitbook/assets/image (66) (1).png>)

#### Delete Rows

This method is used to delete rows from a table in your spreadsheet. First you need to input the range of the table using A1 notation, and then fill the filter that will select the rows that are going to be deleted. If you select the _Use first row as header_ option, the filter can be a JSON object with the keys being the names of the columns, otherwise, they should be JSON objects where the keys are the indexes of the columns in their order.&#x20;

![Examples for deleting all items where the name is Notebook](<../../../.gitbook/assets/image (64) (1) (1).png>)

#### Using parameters in the methods

You can add parameters to your methods, that will be filled in the front end, by adding keywords that begin with a dollar sign. This example updates an item with an id that will be provided by the front end, setting the value to another parameter that will be provided in the front end.

![](<../../../.gitbook/assets/image (55) (1).png>)
