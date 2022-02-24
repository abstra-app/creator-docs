---
description: >-
  When no-code limits you, you can always extend the capabilities of the
  platform using code while keeping the rest of your application visually
  editable.
---

# Expression mode

All arguments have on their top-right corner a `JS` button which toggles it from the stock UI to a text area where the user can write JavaScript code and complex logic.

![](../../../.gitbook/assets/expression-identify.gif)

As the name states, this field expects a JavaScript snippet that will be evaluated as the argument value itself, so the value must fit the expected [argument types](argument-types.md) and range of values (when applicable).

For example, if you set a text value argument of a [text element](../elements/text.md) with expression mode to&#x20;

```
if ($.isLoading) {
    return "Loading";
} else {
    return "Done!";
}
```

the evaluator will check the context object `$` for a `isLoading` [variable](../variables.md) to decide if it is going to display `Loading` or `Done!`. (Yes, that is a ternary operator and they are very frequently used in expressions)

![](<../../../.gitbook/assets/isloading (1).gif>)

There are several other use cases for expression modes, check them out in the section [common techniques](../../../tutorials/common-tecniques/).
