# GraphQL

This connector is used to make requests to GraphQL API.

### Configuration

To configure the connector, simply add the endpoint in the _url_ field and add any header you may need for the request. Then, you can create all the queries and mutations you need by adding new methods to the connector.

![](<../../../.gitbook/assets/image (64).png>)

### Creating queries and mutations

Queries and mutations are the methods of the connector. To make one, simply create a new method and fill the _query_ field. Other optional parameters are _JSON Path_, to parse the response of the API with the [JSON Path](https://jsonpath.com) query language, and the headers parameter, for query-specific headers you may need.

![](<../../../.gitbook/assets/image (60) (1) (1).png>)

### Adding variables to your method

If you wish to add variables to your method, simply add them like you normally would, and fill the variables parameter when using the connector.

![](<../../../.gitbook/assets/image (55).png>)
