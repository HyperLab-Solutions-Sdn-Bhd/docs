{% method %}
# transform(data, lang, apikey)

Dialex takes in a string of words, returning the cleaned up format...
<br>
### Parameters
data - Place your data here. 
(*String*)

lang - Language of given input, 'en' for English, 'ms' for Malay.
(**optional**, **default='en'**)

apikey - This is the unique API key generated from your user profile. *Keep it safe!*
(*String*, **required**)

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

If you prefer to **curl**,

```bash
$ My first method
```


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

status - HTTP response code for the operation.
output - 

{% endmethod %}
