---
description: 'Sometimes, you need to display numbers with distinct formats'
---

# Formating numbers

## Decimal places

If you need set a fixed number of decimal places, you can toggle JS mode and then usd `.toFixed` method from Javascript.

{% hint style="info" %}
The variable/data type should be `number`, otherwise the method `toFixed` will not be available.
{% endhint %}

![Example on adding decimal places on number display](../../.gitbook/assets/formating-numbers-to-fixed.gif)

### Using commas or other formats

Once you are in Javascript mode, you can always replace characters, like that:

```text
$.salary.toFixed(2).replace(/\./g, ',')
```

