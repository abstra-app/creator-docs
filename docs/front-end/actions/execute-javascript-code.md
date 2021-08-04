# Execute JavaScript code

The `Execute JavaScript code` action executes some custom JavaScript code. It lets you control the flow of your actions in case of success or in case an error is thrown.

![](../../../.gitbook/assets/screenshot-from-2021-08-04-13-27-31.png)

You can type some JavaScript code to be evaluated in our code editor.

![](../../../.gitbook/assets/screenshot-from-2021-08-04-13-27-50.png)

Just like our `JS mode` for other arguments, you can reference variables inside your JavaScript code using the `$.` prefix. Example, assuming you have a variable `post` with a `content` property, you can access it as follows:

```javascript
function getPostContent() {
  return $.post.content;
}
getPostContent();
```

You can trigger subsequent actions in case of success or error. The example below shows the message `Success` when the code executes without any errors and shows the message `Error` when the code throws an error.

![](../../../.gitbook/assets/screenshot-from-2021-08-04-13-36-13.png)

