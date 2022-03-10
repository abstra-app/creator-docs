---
description: In this tutorial, we will learn how to make an collapsible sidebar
---

# Collapsible sidebar

[Example](https://create.abstra.app/template/2b3ddcf3-770f-483b-ab0c-c99c3f67b3bf)

First, lets create the two versions of our sidebar (collapsed and expanded).

![We just drew the elements, no components are involved yet](<../../.gitbook/assets/image (71) (1).png>)

Now we can transform each version into one component.

![Each version of the sidebar is now a component](<../../.gitbook/assets/image (49) (1).png>)

{% hint style="warning" %}
Notice that no distances to the right of the page are fixed. This is important because the sidebar is aligned to the left.
{% endhint %}

Now you have both components, you can add a click event on the hamburger menu icon to show the expanded version of the sidebar.

![You only need to trigger the expanded version](<../../.gitbook/assets/image (61) (1) (1).png>)

Now you should have a working sidebar like that:

![Modals come with the default "collapse when click outside" behavior](../../.gitbook/assets/collapsible-sidebar-1.gif)

Notice that the expanded sidebar is shown glued to the top. You can fix that by making an offset on the expanded sidebar with the same size as your navbar

![Just the expaned sidebar should have this offset in px](<../../.gitbook/assets/image (62) (1).png>)

![It should work like this](../../.gitbook/assets/collapsible-sidebar-2.gif)

