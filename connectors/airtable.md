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

![Airtable&apos;s API page](../.gitbook/assets/image%20%2817%29.png)

Select the base you want to connect, then copy the id from URL

![Selecting the application in the Airtable&apos;s API](../.gitbook/assets/get-base-api.gif)

![The base ID in the API URL](../.gitbook/assets/image%20%2822%29.png)

### Generating an API key

You can generate API keys on your [account page](https://airtable.com/account).

![Generating a new API key](../.gitbook/assets/generating-an-api-key.gif)

## Making queries to your base

You can make queries by adding methods.

![Adding a method for Airtable](../.gitbook/assets/adding-method.gif)

After that, you can select the table you want to grab the data

![Choosing a table](../.gitbook/assets/selecting-the-table-name.gif)

Now you can use this connector with Tables, Collections or Actions

## Filtering

Sometimes, you want to filter which elements of Airtable you will want to use. For this, we have a filtering feature.

We will create another method for listing only completed tasks.

![Creating a new task](../.gitbook/assets/create-list-only-completed.gif)

Then we will add the filter property to this method

![Adding a filter property](../.gitbook/assets/adding-a-filter-prop.gif)

Now we can use [Airtable's formula syntax](https://support.airtable.com/hc/en-us/articles/203255215-Formula-field-reference)

![Filter by formula](../.gitbook/assets/addind-filters.gif)

Additionally, you can pass parameters to theses filters.

![Passing parameters](../.gitbook/assets/passing-parameters.gif)

