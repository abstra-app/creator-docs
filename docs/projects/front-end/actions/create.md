# Insert into table

This action is used to insert rows into a [table](../../back-end/tables.md) you have created in the [back-end](../../back-end/).

### Arguments

#### Table

Select the table you are going to insert the data into.  
Type: [tableId](https://docs.abstra.app/docs/projects/front-end/arguments/argument-types#tableid)

#### Values

Input the values of the columns for the row you are creating in the table. This field expects a JSON value in which the keys are the columns names and the values are the values you wish to insert. For example, if you have a table with columns `name` and `age`, and you wish to insert values `John` and `42`, the field should be `{"name": "John", "age": 42}`   
Type: [json](https://docs.abstra.app/docs/projects/front-end/arguments/argument-types#json)

### Outcomes

#### On success

The action you wish to execute after the data is successfully inserted in the database.  The created row is fed into the context as the result variable, accessible through mustache notation as `{{result}}` or in the expression mode as `$.result`

#### On error

The action you wish to execute if something stops the data from being inserted in the database. The query result is fed into the context as the result variable, accessible through mustache notation as `{{result}}` or in the expression mode as `$.result`

