# Load external script

The `Load external script` action loads JavaScript code from a URL to your application. After loading, its lets you control the flow of your actions in case of success or in case an error is thrown.

![](../../../.gitbook/assets/screenshot-from-2021-08-04-14-54-12.png)

You can setup its arguments choosing a `URL` to load the script from and a `Loading type` that can give no feedback to the users of your app or block them from doing anything until the script is loaded.

![](../../../.gitbook/assets/screenshot-from-2021-08-04-14-54-17.png)

A common use case is loading the Google Charts library to create custom charts for your application. Example:

![](../../../.gitbook/assets/chartts.gif)

You can also use it to load a JS library like `lodash` and use it in your custom JS code snippets.

