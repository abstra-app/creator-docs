# Send analytics event

This action helps you integrate events that happen in your application with Google Analytics.

### Arguments

#### Event Action

Name of the event action for the analytics track  
Type: text

#### Event Category

Name of the event category for the analytics track  
Type: text

#### Event Label

Name of the event label for the analytics track  
Type: text

#### Event Value

Value of the event for the analytics track  
Type: number

### Outcomes

#### Success

What happens if everything goes ok with the analytics track  
No additional information is loaded on the context.

#### Fail

What happens if something goes wrong with the analytics track.  
The error is injected on the context for the next action, accessible via `{{error}}` with mustache notation or `$.error` on expression mode.

