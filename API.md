{% method %}
# transform(data, lang, apikey)

Method to transform misspelled text into readable text.
<br>
### Parameters
| Parameters |Info |
| ------------- | ------------- |
| data  | *String*, **required** <br>Place your data here.|
| lang  | *String*, **optional**, **default='en'**<br>Language of given input, 'en' for English, 'ms' for Malay.
 |
| apikey  | *String*, **required** <br>This is the unique API key generated from your user profile. *Keep it safe!*
 |

### Returns
A ```Promise``` containing the response in ```JSON``` format.

<br>

#### Example request
{% sample lang="js" %}
Example usage in **Node**

```js
const Dialex = require('dialex').Dialex;
const dialex = new Dialex('67890cd-testerkey-yz12345');

dialex.transform('my incorect sentense', 'en')
    .then(result => console.log(result))
    .catch(error => console.log(error));
```

If you prefer to **curl**

```bash
$ curl -XGET 'https://dialexherok.herokuapp.com/api/v1/process?data=my%20incorect%20sentense&lang=en&apikey=67890cd-testerkey-yz12345'
```

<br>
#### Example response
``` json
{
    "status": 200,
    "message": "Parse success",
    "output": {
        "result": "my incorrect sentence"
    }
}
```

##### Response object

| Key |Value |
| ------------- | ------------- |
| status  | HTTP response code for the operation.|
| output  | The result of the operation can be found inside ```output.result```|

{% endmethod %}
