{% method %}
# transform(data, lang)

Method to transform misspelled text into readable text.

### Parameters
| Parameters |Info |
| ------------- | ------------- |
| data| *String* (**required**) <br>The string you want to process.|
| lang| *String* (**optional**, **default='en'**)<br>Language of given input, 'en' for English, 'ms' for Malay.|

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

{%sample lang="go" %}
**Go:**  

```go
import "https://github.com/HyperLab-Solutions-Sdn-Bhd/dialex-sdk-go/dialex"

dial := dialex.New("67890cd-testerkey-yz12345")
resp, err := dial.Transform("my incorect sentense", "en")
fmt.Println(resp)
```

{%sample lang="bash" %}
**Curl:**  

```bash
$ curl 'https://dialexherok.herokuapp.com/api/v1/process?apikey=67890cd-testerkey-yz12345&lang=en&data=my%20incorect%20sentense'
```  

{% common %}
#### Response
``` json
my incorrect sentence
```
{% endmethod %}
