{% method %}
# transform(data, lang)

Dialex takes in a string of words, returning the cleaned up format...
<br>
### Parameters
data (*String*)
 - The string you want to process. 

lang (**optional**, **default='en'**)
 - Language of given input, 'en' for English, 'ms' for Malay.

### Returns
A `Promise` containing processed string.

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

#### Example response
``` json
my incorrect sentence
```

{% endmethod %}
