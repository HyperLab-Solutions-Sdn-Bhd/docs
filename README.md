# Getting Started

Setting up Dialex is simple and straightforward. We prepared several SDKs for popular languages and frameworks.

### Node

```js
$ npm install --save @hyperlab-solutions/dialex
```

### **Browser**

```html
<script src="https://cdn.jsdelivr.net/npm/@hyperlab-solutions/dialex/lib/dialex.min.js"></script>
```

## Python

```py
# pip install -U dialex
```

## Quick Start

### NodeJS

```js
const Dialex = require('@hyperlab-solutions/dialex').Dialex;
const dialex = new Dialex('apiKey');
```

### Browser

```js
<script src="https://cdn.jsdelivr.net/npm/@hyperlab-solutions/dialex/lib/dialex.min.js"></script>
...
<script>
let dial = new dialex.Dialex('apiKey');
</script>
```

### Python

```py
from dialex import dialex
dial = dialex.Dialex('apiKey')
```



