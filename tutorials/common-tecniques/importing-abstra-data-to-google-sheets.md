---
description: >-
  Sometimes, you want to have access to your data on google sheets, so
  operational teams can work on top of it. With Abstra APIs, you can easily
  access them.
---

# Importing Abstra data to Google Sheets

## Preparing a query to be executed

After reading [Calling Connectors or Tables from outside Abstra](calling-connectors-or-tables-from-outside-abstra.md). You will be able to have a query to be executed.

## Using Google App Scripts

Google sheets allow javascript-like scripting using their [Google Scripts](https://script.google.com) product. You can easily one script on your spreadsheet by clicking on "Apps Scripts" on the "Extensions" menu.

![Apps script allows you to fetch your data from Abstra APIs](<../../.gitbook/assets/image (49).png>)

After you click in "Apps Script", you should be redirected to a code editor like this

![You can reutilize your scripts across all spreadsheets](<../../.gitbook/assets/image (66).png>)

Here is an example of a script for inserting the result of one query into the spreadsheet

```java
function getDataFromAbstra() {
  const response = UrlFetchApp.fetch(
    "https://tables.abstra.cloud/execute/{{{ QUERY ID TO BE EXECUTED }}",
    {
      headers: {
        "Content-Type" : "application/json",
        "Authorization": "Bearer {{YOUR TOKEN SHOULD COME HERE}}",
      },
      method: "post"
    }
  );

  const records = JSON.parse(response.getContentText());
  const columns = Object.keys(records[0]);
  const rows = records.map(record => columns.map(column => record[column]));

  Logger.log(columns);
  Logger.log(rows);


  const sheet = SpreadsheetApp.getActiveSheet();
  sheet.clear();
  sheet.getRange(1, 1, 1, columns.length).setValues([columns]);  
  sheet.getRange(2, 1, rows.length, columns.length).setValues(rows);  
}
```

{% hint style="info" %}
Notice that this script will replace the active sheet with the data you fetched. Make sure to adapt this script to your needs
{% endhint %}

{% hint style="warning" %}
Notice that you should add your query id and authentication tokens. See [how you can do it](calling-connectors-or-tables-from-outside-abstra.md)
{% endhint %}

