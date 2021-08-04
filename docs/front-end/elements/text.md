# Text

This element lets you show rich text.   
Common uses are titles, text content and descriptions.

![](../../../.gitbook/assets/text.gif)

### Arguments

#### Text Value

Text that will be displayed on the slot.  
Format: [richText](https://docs.abstra.app/docs/front-end/arguments/argument-types#richtext)  
Default: `this is a text`

#### Font Size

Size of the font that will be displayed on the slot.  
Format: [number](https://docs.abstra.app/docs/front-end/arguments/argument-types#number)  
Default: `16`

#### Font Color

Color of the font that will be displayed on the slot.  
Format: [color](https://docs.abstra.app/docs/front-end/arguments/argument-types#color)  
Default: `#000000`

#### Line Height

Height of a line that will be displayed on the slot.  
Format: [number](https://docs.abstra.app/docs/front-end/arguments/argument-types#number)  
Default: `1.5`

#### Alignment

Text alignment inside the slot.  
Format: [alignment](https://docs.abstra.app/docs/front-end/arguments/argument-types#alignment)  
Default: `center`

#### Font Style

Font families for the element. Options are [CSS font-family](https://www.w3schools.com/cssref/pr_font_font-family.asp) properties.

Format: discrete [text](https://docs.abstra.app/docs/front-end/arguments/argument-types#text)  
Default: "Roboto", sans-serif

### Events

The following are the events triggered by this element:

#### On click

When this element is clicked, a `click` event is triggered and actions with this trigger will be initiated. No additional information is loaded on the context.

