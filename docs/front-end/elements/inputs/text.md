# Text

Text inputs are basic single line text inputs for your application. They are commonly used when building forms.

![](../../../../.gitbook/assets/screenshot-from-2021-08-26-11-33-23.png)

&#x20;A text input configuration is divided in 3 different sections. In the first section you can configure it's dimensions, position, responsivity and all of it's arguments.

![](../../../../.gitbook/assets/screenshot-from-2021-08-27-11-36-56.png)

Since `Dimensions`, `Position` and `Responsivity` are common to all elements, you can checkout more about how they work [here](../).

The `Variable` argument is useful for binding an input value to a variable of your application. `Tab Index` and `Accessibility Label` are used to configure how screen readers interact with your application. Other than this default arguments, you can also configure if the input is `Disabled`, a input value `Validation` and if it has an `Emoji Keyboard`.

![](../../../../.gitbook/assets/screenshot-from-2021-08-27-11-42-33.png)

The  second configuration section let's you change you input styles. You can change it's `Background`, `Shadow`, `Border` and `Inner Padding`.

![](../../../../.gitbook/assets/screenshot-from-2021-08-27-11-38-03.png)

Except for the `Inner Padding`, you can change the styles based on user interaction. They all have a `Standard` state configuration but you can change styles during `Hover` and `Click` interactions as well.

![](../../../../.gitbook/assets/screenshot-from-2021-08-27-11-38-27.png)

The  third configuration section let's you change you input `Placeholder`.

![](../../../../.gitbook/assets/screenshot-from-2021-08-27-11-40-13.png)

## Masks

You can customize the acceptable format of each input by using masks

![Mask is a optional parameter, so you have to add on the + button](<../../../../.gitbook/assets/image (53) (1) (1).png>)

Examples of masks:

`00/00/0000` for dates

`(000) 000 - 0000` for US phone numbers

`aaa` for currency codes

And you can also have multiple masks on the same input by writing pipes | between them and the input value will adjust based on text length

(PATTERN-A)|(PATTERN-B)|(PATTERN-C)

Example: 000.000.000-00|00.000.000/0000-00
