{% method %}
# transform(data, lang)

Method to transform misspelled text into readable text.

### Parameters
| Parameters |Info |
| ------------- | ------------- |
| data| *String* (**required**) <br>The string you want to process.|
| lang| *String* (**optional**, **default='en'**)<br>Language of given input, 'en' for English, 'ms' for Malay.|

### Returns
A ```Promise``` containing the processed sentence.


{% common %}
#### Example request

{% sample lang="js" %}
Usage:

```js
const Dialex = require('@hyperlab-solutions/dialex').Dialex;
const dialex = new Dialex('67890cd-testerkey-yz12345');

dialex.transform('my incorect sentense', 'en')
    .then(result => console.log(result))
    .catch(error => console.log(error));
```

{% common %}
#### Example response
``` json
my incorrect sentence
```
{% endmethod %}
