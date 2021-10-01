# Conditional rendering

You can use subviews to conditionally render components in your application. Add a [Reutilized Component](../../docs/front-end/elements/subview.md) to your page.

![](../../.gitbook/assets/screen-shot-2021-10-01-at-14.05.45.png)

In this example we are going to use a `isHappy` variable to conditionally render some component.

![](../../.gitbook/assets/screen-shot-2021-10-01-at-14.07.44.png)

Then we can bind this variable to a [Checkbox Input](../../docs/front-end/elements/inputs/checkbox.md)  just to toggle our variable and test our conditional render.

![](../../.gitbook/assets/screen-shot-2021-10-01-at-14.10.13.png)

Now we can toggle our [Reutilized Component](../../docs/front-end/elements/subview.md) based on this variable value. We just have to bind our components to some reference and add a ternary expression in your [JS mode](../../docs/front-end/arguments/expression-mode.md) to choose between our references based on the `isHappy` variable value.

![](../../.gitbook/assets/screen-shot-2021-10-01-at-14.11.42.png)

Working example:



