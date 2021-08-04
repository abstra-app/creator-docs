# Hosted Tables

The `Hosted Tables` action is used to dispatch one `query` defined at the `Hosted Tables` division of Abstra's `Backend` section.

![](../../../.gitbook/assets/screenshot-from-2021-08-04-18-04-35.png)

You can choose a `SQL Query` to be executed and a `Loading type` that can give no feedback to the users of your app or block them from doing anything until the query finishes executing. If your query has parameters defined you can pass values directly or through variables.

![](../../../.gitbook/assets/screenshot-from-2021-08-04-18-04-57.png)

After the query execution a `data` and an `error` variables will be exposed and can be used to do operations with other actions. The example below displays the message `Success` with the `data` in case of a successful execution and the message `Error` with the `error` in case of a failed execution of the `getPosts` query. 

![](../../../.gitbook/assets/screenshot-from-2021-08-04-18-05-50.png)

