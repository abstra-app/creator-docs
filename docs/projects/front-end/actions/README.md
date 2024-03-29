# Actions

Actions are how you add interactivity to your application. You can attach actions to certain events in your elements or views, and use them to interact with the user through the GUI or communicate with a back-end application.

An action has: **arguments**, which describe its behavior and are much like an [element'](../elements/)s arguments; **outcomes,** which are events generated by the action, that can trigger other actions much like the element's events, and each outcome can feed variables into the next action's context. If an outcome feeds the variable `foo` into it's context, it will be accessible in the triggered action's context by using mustache notation `{{ foo }}` or in the expression mode `$.foo`

### Reuse and Reordering

Actions can be reordered and reused. Just drag its trigger pills and delete obsolete triggers.

![](../../../../.gitbook/assets/reorder-actions.gif)

These are the actions and their description:

