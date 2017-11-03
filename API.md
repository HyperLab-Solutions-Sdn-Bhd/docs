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
#### Example

{% sample lang="js" %}
**NodeJS:**

```js
const Dialex = require('@hyperlab-solutions/dialex').Dialex;
const dialex = new Dialex('67890cd-testerkey-yz12345');

dialex.transform('my incorect sentense', 'en')
    .then(result => console.log(result))
    .catch(error => console.log(error));
```  

**Browser**  

```js
<script src="https://cdn.jsdelivr.net/npm/@hyperlab-solutions/dialex/lib/dialex.min.js"></script>
...
<script>
let dial = new dialex.Dialex('67890cd-testerkey-yz12345');
dial.transform('my incorect sentense', 'en')
    .then(result => console.log(result))
    .catch(error => console.log(error));
</script>
```  

{%sample lang="python" %}
**Python:**  

```python
from dialex import dialex

dial = dialex.Dialex('67890cd-testerkey-yz12345')
resp = dial.transform('my incorect sentense', 'en')
print resp
```

{% common %}
#### Response
``` json
my incorrect sentence
```
{% endmethod %}
