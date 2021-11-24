---
description: >-
  Airtable is a spreadsheet-database hybrid, with the features of a database but
  applied to a spreadsheet
---

# Airtable

## Connecting to Airtable

In order to get data from Airtable, you should have the following information in hand

* Base ID
* API key

### Getting base ID

Visit [https://airtable.com/api](https://airtable.com/api), then you should see something like this

![Airtable's API page](<../../../.gitbook/assets/image (17).png>)

Select the base you want to connect, then copy the id from URL

![Selecting the application in the Airtable's API](../../../.gitbook/assets/get-base-api.gif)

![The base ID in the API URL](<../../../.gitbook/assets/image (22).png>)

### Generating an API key

You can generate API keys on your [account page](https://airtable.com/account).

![Generating a new API key](../../../.gitbook/assets/generating-an-api-key.gif)

## Making queries to your base

You can make queries by adding methods.

### List Records

![Adding a method for Airtable](../../../.gitbook/assets/adding-method.gif)

After that, you can select the table you want to grab the data

![Choosing a table](../../../.gitbook/assets/selecting-the-table-name.gif)

Now you can use this connector with Tables, Collections or Actions

#### Filtering

Sometimes, you want to filter which elements of Airtable you will want to use. For this, we have a filtering feature.

We will create another method for listing only completed tasks.

![Creating a new task](../../../.gitbook/assets/create-list-only-completed.gif)

Then we will add the filter property to this method

![Adding a filter property](../../../.gitbook/assets/adding-a-filter-prop.gif)

Now we can use [Airtable's formula syntax](https://support.airtable.com/hc/en-us/articles/203255215-Formula-field-reference)

![Filter by formula](../../../.gitbook/assets/addind-filters.gif)

Additionally, you can pass parameters to theses filters.

![Passing parameters](../../../.gitbook/assets/passing-parameters.gif)

#### Additional properties

![](../../../.gitbook/assets/airtable-others.gif)

Other properties you can define are:

* **Maximum number of records**. Specify this to limit the number of records returned
* **List of fields to return**: Specify which fields you want to query.
* **List of fields to sort**: Specify fields and directions to order your query.
* **Include Record ID**: A boolean value to decide if the record id should be included in the result fields

### Create One Record

Here you can create one record on a table. There are 3 possible arguments:

* **table**: Name of the table from where you will be fetching data from. Same as in the **list records** method.
* **fields**: A JSON template (it supports named params like _$params_) to insert in the database
* (optional) **include Record Id**: A boolean value to decide if the record id should be included in the result fields.

![](../../../.gitbook/assets/create-air.gif)

### Update Record

Here you can create one record on a table. There are 3 possible arguments:

* **table**: Name of the table from where you will be fetching data from. Same as in the **list records** method.
* **fields**: A JSON template (it supports named params like _$params_) to insert in the database
* (optional) **include Record Id**: A boolean value to decide if the record id should be included in the result fields.

During the use of this method the ID parameter will be prompted. This parameter is required by AirTable to update the specific record. In order to use this the user must have requested (or saved) the ID in a prior action. To get this ID you must toggle on the _includeRecordId_ parameter in the method that retrieves the record data.

![](../../../.gitbook/assets/update-air.gif)
