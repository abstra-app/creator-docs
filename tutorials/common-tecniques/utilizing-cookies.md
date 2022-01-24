---
description: Here we will show you a quick way to utilize the cookies from your browser.
---

# Utilizing Cookies

First of all we need to create a new `Execute Javascript code` Action.&#x20;

![Creating a new Execute Javascript code Action](<../../.gitbook/assets/Screen Shot 2022-01-24 at 18.12.36.png>)

That way we can utilize the Javascript to reach the cookies from the Browser by calling the method `document.cookie`. Like shown below.

![Simple JS code that'll retrieve the cookies](<../../.gitbook/assets/Screen Shot 2022-01-24 at 18.18.02.png>)

Now we could utilize that cookie we just returned in any other action with the then trigger and `$.returnValue`. Such as on the `Show Message` Action.

![Utilizing the return on another action](<../../.gitbook/assets/Screen Shot 2022-01-24 at 18.18.18.png>)

Now the only problem remaining is that `document.cookie` returns a string which can be quite troublesome to manipulate sometimes. So lets convert it to an object that'll be ready to be used or setted into a variable.

![Here we added the parseMyCookie function to our code and call it on getBrowserCookies in order to get our cookies in an object.](<../../.gitbook/assets/Screen Shot 2022-01-24 at 18.49.22.png>)

```
function parseMyCookie(str) {
    str = str.split('; ');
    var result = {};
    for (var i = 0; i < str.length; i++) {
        var cur = str[i].split('=');
        result[cur[0]] = cur[1];
    }
    return result;
  }
```

Finally we just need to add something to actually call the javascript code.\
Let's say we use a press of a button, that is, the trigger On Click of our Button.

![Here we created the button and dragged the on click trigger to our action.](<../../.gitbook/assets/Screen Shot 2022-01-24 at 18.18.38.png>)

Now we're ready to go. :)

![Click on the button will show our cookies. :)](<../../.gitbook/assets/cookie gif.gif>)
