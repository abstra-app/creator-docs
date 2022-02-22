# REST v2

Our REST v2 connector is suited for connecting with **HTTP REST APIs** in a more secure manner.

In order to use it, you should fill the _base url_ with the base endpoint.

For example, if you want to connect to the endpoints **https://myapi.com/some-data** and **https://myapi.com/some-other-data**, then the _base url_ would be **https://myapi.com**

![](<../../../.gitbook/assets/image (70).png>)

You can also set connector-wide headers to be sent with all methods. Note that method headers can overwrite connector headers with the same key.

### **About Security**

This connector can be executed from our servers or from your users browser.&#x20;

* **Local Request**: executing from the users browser can be useful when user specific params or network settings are required such as IP address blocks. But be aware that because the request is leaving the users browser all the configured params (headers, body) are publicly accessible.&#x20;
* **Remote Request**: executing from our servers masks user specific params or network settings such as IP addresses. On the other hand, as all requests are leaving our servers, most of the params are not publicly available, so you can configure secrets such as api keys in headers or body

### Methods

The methods are used to connect to the actual endpoints in your **API**.

You can make GET, POST, PUT and any other HTTP method requests.

#### **Route Parameters**

You can add **route parameters** with ":" before the param:

```
/myroute/:myRouteParam
```

If you use route parameters, the necessary arguments will be requested when calling the method on the frontend.

**Body Parameters**

If you are sending a request that needs a body, you can set a template of the body and just fill the dynamic fields. You can add **body parameters** with "$" inside the field:

```json
{
	"name": $name,
	"age": $age
}
```

**Header Parameters**

If you are sending a request that needs a authorization or just need to pass params in the headers, you can create params inside the headers with "$" inside the field:

```
Authorization: Bearer $token
```
