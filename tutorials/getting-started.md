# Getting started

The first time you create a project, you see this screen.

![Interface map](../.gitbook/assets/interface.png)

## Components picker

This is your main utility toolbelt. Drag the components on the interface to use them.

![](../.gitbook/assets/drag-to-add-components.gif)

## Canvas

This is the area where you build and see your project. Within this area, you can pan and zoom to move around.

### Pan

![Pan movement](../.gitbook/assets/pan.gif)

* Space + drag
* Middle-click + drag
* Scroll \(vertical\)
* Shift + scroll \(horizontal\)
* Two fingers swipe

### Zoom

![Zoom](../.gitbook/assets/zoom.gif)

* Ctrl + Scroll

## View frame

This is where you create your layouts. It can be a page or a component. The mechanics depend on your layout engine setup \(at the beginning of the project\).

### Elastic

Main mechanics:

![Click to select a compoent](../.gitbook/assets/select.gif)

![Shift + click to add to selection](../.gitbook/assets/shift-select.gif)

![Shift + click to unselect](../.gitbook/assets/shift-unselect.gif)

![Draw a rectangle to select](../.gitbook/assets/rectangle-select.gif)

![Drag to move](../.gitbook/assets/translate.gif)

![Shift + drag to restrict movement vertically/horizontally](../.gitbook/assets/shift-drag.gif)

![Alt + drag to duplicate](../.gitbook/assets/alt-translate.gif)

![Corners to resize](../.gitbook/assets/resize%20%281%29.gif)

![Shift + resize to maintain proportions](../.gitbook/assets/shift-resize.gif)

![Alt + resize to maintain simetry](../.gitbook/assets/alt-resize.gif)

![Resize + drag in multiple elements](../.gitbook/assets/multiple-transform.gif)

### Flex

![Add elements by dragging](../.gitbook/assets/add-first-element-by-drag.gif)

![Add elements on sides](../.gitbook/assets/add-elements-on-the-side.gif)

![Resize elements on the side](../.gitbook/assets/flex-resize.gif)

![Select ancestor elements in the lower breadcrumb](../.gitbook/assets/hover-to-tree.gif)

![Each node has a direction different from its parent](../.gitbook/assets/alternate-directions.gif)

#### Size types

each flex slot have 3 options of size types

![Size types editor](../.gitbook/assets/image%20%2824%29.png)

**Expand**

This makes the slot expand proportionally to its parent. Measured in %, this is great for content containers, blank areas, and other non-functional slots.

![Expand size type](../.gitbook/assets/expand.gif)

**Fixed-size**

This size type makes the size fixed in pixels, no matter its parent's size. Measured in pixels, this is great for navbars, sidebars, footers, and other navigation elements.

![Fixed size type](../.gitbook/assets/fixed%20%281%29.gif)

**Fit to content**

This size type makes the size equal to the minimum required by its content. This cannot be resized once is defined by its content only. Great for buttons, inputs, and other components in the interface.

![Fit to content](../.gitbook/assets/content-fit.gif)

## Actions

When you want any kind of logic on your application, you need actions. This feature allows you to call APIs, change pages, etc.

![Click to add actions](../.gitbook/assets/actions-click-to-add.gif)

![Select an action](../.gitbook/assets/actions-click-to-select.gif)

![Select what you want to do](../.gitbook/assets/actions-select-type.gif)

![Actions can be dispatched from multiple types of triggers](../.gitbook/assets/actions-multiple-triggers-possible.gif)

![Drag to reutilize actions](../.gitbook/assets/actions-drag-to-reutilize.gif)

![Views can have actions too](../.gitbook/assets/actions-views-have-actions.gif)

![Actions can have actions as well](../.gitbook/assets/actions-actions-have-actions.gif)

![Triggers can be selected too](../.gitbook/assets/actions-select-trigger.gif)

![Delete actions](../.gitbook/assets/actions-delete.gif)

## Project inspector

This is where you can see the entities of your projects.

### Pages

![show pages](../.gitbook/assets/project-inspector-pages.gif)

![add page](../.gitbook/assets/project-inspector-add-page.gif)

![rename page](../.gitbook/assets/project-inspector-rename-page%20%281%29%20%281%29.gif)

![delete page \(need confirmation\)](../.gitbook/assets/project-inspector-delete-page.gif)

### Components

These are the reutilized elements on your interface. You can use them for navbars, sidebars, footers, cards, and other repeated pieces of the layout.

![Components tab](../.gitbook/assets/components.gif)

![Add component](../.gitbook/assets/components-add-component.gif)

![Rename component](../.gitbook/assets/components-click-to-rename.gif)

![Delete component](../.gitbook/assets/components-delete-component.gif)

### Global variables

See [variables](../docs/front-end/variables.md).

See [Local variables](getting-started.md#local-variables).

Variables are used to coordinate your application state. Just like in programming.

In Abstra, global variables are shared across the navigation.

![Global variables tab](../.gitbook/assets/variables.gif)

![add global variable](../.gitbook/assets/variables-add-variable.gif)

![Edit variable](../.gitbook/assets/edit-variable.gif)







## Selection inspector

This is the area where you can edit what is selected on the canvas.

![Selection inspector changes depending on what is selected](../.gitbook/assets/selection-inspector.gif)

## View inspector

This is the area where you can navigate through the entities of your view \(page or component\).

### View settings

![View settings](../.gitbook/assets/view-inspector-details.gif)

### Local variables

See [variables](../docs/front-end/variables.md).

Variables are used to coordinate your application state. Just like in programming.

In Abstra, local variables live in one view \(page or component\).

See[ Global variables](getting-started.md#global-variables).

## Project tabs

![Use this tabs to access your backend and settings page](../.gitbook/assets/project-tabs.gif)

### Frontend

This is the face of your application. This part contains the layout where your users can interact directly through the interface.

### Backend

This is the part where your users don't touch directly, this is where you store your data, send emails, access other APIs.

### Settings

General settings of your projects. In this part, you can change the project name, configure auth, and other global parameters.

## Breadcrumb navigation

You can use to navigate to your workspaces or rename the project.

![Click to rename](../.gitbook/assets/rename-project.gif)

## Project toolbar

![Project toolbar](../.gitbook/assets/image%20%2825%29.png)

### Chat

Use this chat to talk with our staff whenever you have any problems or questions about Abstra.

### Docs

This link brings to these docs \(where you are reading right now\)

### Preview

Allows you to simulate your application running, so you can easily debug what is happening

### Publish

Generate a version of your app online, so you can test it with a shareable link with your teammates.

