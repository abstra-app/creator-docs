---
description: Lists important changes to the editor
---

# Changelog

## 2022/03/13 - 2022/03/19

* Added AWS WorkMail to our [email connector](docs/back-end/connectors/e-mail.md)
* Added [Listing of elements](https://docs.abstra.app/docs/front-end/elements/elements-list) in a page/component
* Added folders to components

## 2022/03/06 - 2022/03/12

* Added new block screen type in some actions: [call connector](docs/front-end/actions/call-connector.md), [execute statement](docs/front-end/actions/hosted-tables.md), [load script](docs/front-end/actions/load-external-script.md), [upload file](docs/front-end/actions/upload-file.md) and [api login](docs/front-end/actions/sign-in-with-username-password.md). You can now show a loading indicator that blocks the screen until the action flow is over.
* Now we show logs of previous runs on triggers, actions an expressions
* Added filter on page / component list
* Added a global search for Pages/Components/Statements/Connectors/Methods

## 2022/02/20 - 2022/02/26

* Added color, rich text and datetime options for variable types
* Added [restv2](docs/back-end/connectors/rest-v2.md) connector
* Now you can share templates
* [Expression](docs/front-end/arguments/expression-mode.md) mode is smarter and accepts both return and expression statements
* We've changed our [code editor](docs/front-end/code-editor.md) in order to give you more readability and life qualities when you're in need of writing down that piece of code.

## 2022/02/13 - 2022/02/19

* Adding option on text input of multiple [masks](https://docs.abstra.app/docs/front-end/elements/inputs/text)
* New action layout with better context

## 2022/02/06 - 2022/02/12

* Adding after [loop event](https://community.abstra.app/news-9a282l1t/post/feature-improvement-after-loop-event-2DAa9kx9Isiwd2I)

## 2022/01/30 - 2022/02/05

* Added Cc and Bcc fields to [email connector](docs/back-end/connectors/e-mail.md)

## 2022/01/23 - 2022/01/29

* Lots of bug fixes and internal improvements to make our product more robust

## 2022/01/16 - 2022/01/22

* Bug fix week
* Add option for more fonts, weights and style

## 2022/01/09 - 2022/01/15

* Now you can edit, add and remove spring and breakpoints of multiple elements at once
* We now have support for [breakpoints](docs/front-end/breakpoints.md)
* Bug fix week

## 2022/01/02 - 2022/01/08

* Bugfix: handling error when variable's type points to a deleted table. Now we display a message informing this.
* Added an alternative for popup login: [Redirect Login](docs/front-end/actions/redirect-sign-in-sign-up.md).&#x20;
* Added option to choose item overflow for collection

## 2021/12/26 - 2022/01/01

* Adding [input masks](docs/front-end/elements/inputs/text.md#masks).
* Bugfix: allowing empty numeric inputs.
* [New modal mechanics](docs/front-end/actions/show-modal.md#customization-with-springs).

## 19/12/2021 - 25/12/2021

* Added Breakpoints functionality;

## 28/11/2021 - 04/12/2021

* Change the default behaviour of the upload method on the storage connector: now you need to opt-in to add a hash to the filename
* Add Code connector with the first method: Python Code!

## 21/11/2021 - 27/11/2021

* Added create and update methods to Airtable connector
* Now you can see who is online with you in your project when you are editing
* invalid iframe sources will no longer render the current page
* fixed a bug that allows you to paste images while in preview mode
* Better table typing, including list of rows. Also added List and Object types.

## 16/11/2021 - 19/11/2021

*   Now you can turn your projects into templates. Utilize that project you have as a base for other new applications you wanna build!&#x20;

    We also will be releasing more and more templates curated by Abstra so you can get your projects out of the box faster.
* Fixed some bugs with group duplication

## 07/11/2021 - 13/11/2021

* We introduced the new access rule feature that simplifies granular access control of some assets in your application. Learn more in [access control](docs/project-settings/authentication.md#access-rules) or this [lesson](tutorials/common-tecniques/auth0-roles.md#using-roles-in-abstra)

## 31/10/2021 - 06/11/2021

* Now you are able to configure your elements responsivity at the right sidebar.

## 24/10/2021 - 30/10/2021

* Now you have group mechanics to deal with your frontend elements;
* Hosted Tables queries now accept named parameters.

## 17/10/2021 - 23/10/2021

* Now you can add params to the prefixes of storage connector;
* Now you can edit buttons when double clicking them;
* We added number type to our text input;
* We added events to our modal, now you can listen to an event through your modal;
* Fixed some pesky bugs within editing inputs;
* Fixed our checklist not inputing when checking a box.



## 10/10/2021 - 16/10/2021

* Now when you clone a page or component, the new one will have the original name plus `- copy`

## 03/10/2021 - 09/10/2021

* [Components](docs/front-end/components.md) can emit events and [subview](docs/front-end/elements/subview.md) elements can handle emitted elements with actions;
* Action [external link](docs/front-end/actions/external-link.md) can open in same tab;
* Date picker allows more format options;
* Inputs now accepts double clicks to edit the placeholder (Only on those where this applies, for instance checklist don't have this function); &#x20;
* Now when you select "add all fields" on the query builder, it will remain highlighted and new columns will be added to the result (equivalent to "\*" on SQL).

## 26/09/2021 - 02/10/2021

* New design for backend (connectors + tables);
* New hints on how to build your apps using Abstra;
* Fixed rendering bug after changing pages or components;
* When you reload the page, the state of the locks are preserved;
* Fixed an issue with arguments re-rendering queries;
* Reload element methods for table and collection are back;
* Fixed an issue with special chars in postgres connection string;&#x20;
* Now when componetizing your elements together, those on the border will receive a spring automatically in order to preserve the resposivity.

## 19/09/2021 - 25/09/2021

* Now you can add members to your workspace that are not yet enrolled with Abstra;
* New [live example](https://youtu.be/g7zXapUv\_ik);
* New users will receive a welcome email with useful information;
* Fix some bugs with page or components names;
* Expression editor popup now remembers its position;
* Projects open in the last opened view or the first.

## 12/09/2021 - 18/09/2021

* We are happy to announce that the [Google Sheets Connector](docs/back-end/connectors/google-sheets.md) is now on Beta;
* Now when you press alt while dragging a component and release the mouse button it will duplicate your component. (Before it would only do so if you were pressing alt at the start of the click);
* Fixed the bug related to style arguments showing a default value when disabled;
* Fixed the bug related to the color input changing the color to black randomly;
* Added an option to set the first row as a header in the Get Range method of [Google Sheets Connector](docs/back-end/connectors/google-sheets.md);
* Added a Storage Connector to allow you to upload and list files from a storage provider.
