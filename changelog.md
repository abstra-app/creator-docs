---
description: Lists important changes to the editor
---

# Changelog

## 03/10/2021 - 09/10/2021

* [Components](docs/front-end/components.md) can emit events and [subview](docs/front-end/elements/subview.md) elements can handle emitted elements with actions
* Action [external link](docs/front-end/actions/external-link.md) can open in same tab
* Date picker allows more format options
* Inputs now accepts double clicks to edit the placeholder \(Only on those where this applies, for instance checklist don't have this function\).  
* now when you select "add all fields" on the query builder, it will remain highlighted and new columns will be added to the result \(equivalent to "\*" on SQL\)

## 26/09/2021 - 02/10/2021

* New design for backend \(connectors + tables\)
* New hints on how to build your apps using Abstra
* Fixed rendering bug after changing pages or components
* When you reload the page, the state of the locks are preserved
* Fixed an issue with arguments re-rendering queries
* Reload element methods for table and collection are back!
* Fixed an issue with special chars in postgres connection string 
* Now when componetizing your elements together, those on the border will receive a spring automatically in order to preserve the resposivity.

## 19/09/2021 - 25/09/2021

* Now you can add members to your workspace that are not yet enrolled with Abstra
* New [live example](https://youtu.be/g7zXapUv_ik)
* New users will receive a welcome email with useful information
* Fix some bugs with page or components names
* Expression editor popup now remembers its position
* Projects open in the last opened view or the first

## 12/09/2021 - 18/09/2021

* We are happy to announce that the [Google Sheets Connector](docs/back-end/connectors/google-sheets.md) is now on Beta;
* Now when you press alt while dragging a component and release the mouse button it will duplicate your component. \(Before it would only do so if you were pressing alt at the start of the click\);
* Fixed the bug related to style arguments showing a default value when disabled;
* Fixed the bug related to the color input changing the color to black randomly.
* Added an option to set the first row as a header in the Get Range method of [Google Sheets Connector](docs/back-end/connectors/google-sheets.md)
* Added a Storage Connector to allow you to upload and list files from a storage provider.

