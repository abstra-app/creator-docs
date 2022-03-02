# Code

With this connector you can run code on our trusted remote servers.

At this momento we only support the python programming language.

### Python

You can write regular python 3.8 scripts commands here, for example:

```python
import requests

r = requests.get("https://create.abstra.app/version.json")
output_data = r.json()
```

{% hint style="warning" %}
The runtime is Python 3.8, the memory usage limit is 128MB and and the execution will timeout after 10 seconds if it is not over yet.
{% endhint %}

#### **About input and output**

To feed data to your code you need to use the `input` param. In it you can specify any JSON-like value (dictionaries, arrays, strings) and even use named params to dynamically fill values. This param is injected into the local context of your code and can be accessed with the `input_data` variable.

To return data, just create a variable called output\_data its value will be returned (it needs to be serializable).

For example, the following method passes an object with a key `num` as the `input_data` and has the `$num` param; The `output_data` is the squares of integers smaller then the input:

![](<../../../.gitbook/assets/image (64) (2).png>)

And can be used like this:

![](<../../../.gitbook/assets/image (59) (1) (1) (1).png>)

About `imports`

{% hint style="warning" %}
Importing python modules is currently limited to the `requests` package. Others will be available in the future.
{% endhint %}

You can import modules (currently only requests) and use it normally:

![](<../../../.gitbook/assets/image (60) (1) (1) (1) (1) (1).png>)

#### Running Async

If you tick the box "run asynchronously" your method will return `running async` and don't wait for the code to finish. Otherwise it will wait for the code to finish before returning the `output_data`



