# Upload file

The `Upload file` action is used to upload a single or multiple files.

![](../../../.gitbook/assets/screenshot-from-2021-08-04-15-25-14.png)

You can setup its arguments choosing a `File type` that will be uploaded, a `File amount` and a `Loading type` that can give no feedback to the users of your app or block them from doing anything until all files are uploaded.

![](../../../.gitbook/assets/screenshot-from-2021-08-04-15-25-18.png)

You can trigger subsequent actions in case of success or error. The example below shows the message `Success` when the upload executes without any errors and shows the message `Error` when the upload throws an error. The `error` variable will be exposed in case of an error and a `file` or `files` variable will be exposed in case of a success, depending it its a single or multiple files upload.

![](../../../.gitbook/assets/screenshot-from-2021-08-04-15-30-59.png)

