# For each

The `For each` action is used to fire another action for each item of a specified list.

![](../../../.gitbook/assets/screenshot-from-2021-08-04-17-48-19.png)

You can choose a `List to iterate` that can be manually defined in the action or reference an existing variable toggling it's value to JS mode.

![](../../../.gitbook/assets/screenshot-from-2021-08-04-17-48-33.png)

Every iteration or failure exposes an `item` and an `index` variable that can be used to do operations with other actions. The example below displays the message `Success` with the iteration `index` and `item` in case of a successful iteration and the message `Error` with the iteration `index` and `item` in case of a failed iteration. 

![](../../../.gitbook/assets/screenshot-from-2021-08-04-17-51-45.png)

