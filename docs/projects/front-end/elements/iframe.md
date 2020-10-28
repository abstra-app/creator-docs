# iframe

This component lets you render external pages with its embed URL

![](../../../../.gitbook/assets/iframe.gif)

### Arguments

#### **Source**

Description: Iframe source URL  
Type: text  
Default: Area 51 map in Google Maps 

#### **Allow full screen**

Description: Can this iframe be used in full screen?  
Type: boolean  
Default: `false`

### Methods

There is no method available for this component.

### Events

The following are the events triggered by this component:

#### On **message**

When messages are sent by `postMessage`, a `message` event is triggered and actions with this trigger will be initiated.   
The message is injected on the event property on the context, accessible via `{{event}}` with mustache notation or `$.event` on expression mode.

