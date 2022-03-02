---
description: >-
  When drawing your interfaces, you can specify how  your app should look like
  in different devices
---

# Responsivity

## Default behavior

By default, any element will keep its size and position relative to the top-right corner of the view.

![Notice that the navbar bottom is not always aligned to the view bottom](../../.gitbook/assets/default-responsivity.gif)

## Springs

In Abstra, you can fix distances on the interface using springs which allow you to set responsive behaviors on your elements.

### Adding springs

#### Hooks

![Hooks between element and view](../../.gitbook/assets/hook.gif)

![Hooks between elements](../../.gitbook/assets/hook-element-element.gif)

#### Spring shooter

Using the spring shooter in the responsivity inspector tab, you can add springs on the interface without having to manually drag and drop them.

![](<../../.gitbook/assets/image (71).png>)

![Spring shooter allows you to add springs very fast](<../../.gitbook/assets/spring shooter.gif>)

### Behavior

#### Fixing an element to the view

![You can fix elements to the right of the view by using the spring shooter or anchoring the spring to the side.](../../.gitbook/assets/01-fixing-right.gif)

#### Chaining elements

![Chaining elements allows you to fix their position relative to the view, in this case, to the top right corner.](../../.gitbook/assets/02-chaining-elements.gif)

#### Fixing an element to both sides makes it stretch (when not fixed-width)

![By fixing boths sides of an element you can make it stretch with the view.](../../.gitbook/assets/03-fix-elem-both-notfixed.gif)

#### Fixing an element to both sides centers it (when fixed width)

![Fixing both sides of the element and setting it to fixed width allows the element to keep centered in the view.](../../.gitbook/assets/04-fix-elem-both-fixwid.gif)

#### Two columns, both flexible

![Anchoring both elements with springs will make them both flexible, changing their size according to the size of the view.](../../.gitbook/assets/05-2col-bothflex.gif)

#### Two columns, both fixed

![When setting both elements to fixed width, when resizing, both will retain their original sizes.](../../.gitbook/assets/06-2col-bothfixed.gif)

#### Two columns, one flexible, and one fixed

![Having two distinct elements and one of them having a fixed width, only one of them will retain their original size while the other will resize accordingly.](../../.gitbook/assets/07-2col-flexandfixed.gif)

#### Components to make elements fixed amongst themselves

![You can make a component inside another component, using the springs to constrain how these components behave.](../../.gitbook/assets/08-comp-fixed-inbetween.gif)

You can always combine springs and [breakpoints](../../docs/front-end/breakpoints.md) to make fully responsive apps

