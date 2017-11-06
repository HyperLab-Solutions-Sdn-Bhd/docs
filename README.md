# Getting Started

Setting up Dialex is simple and straightforward. We prepared several SDKs for popular languages and frameworks.

### Node

```bash
$ npm install --save @hyperlab-solutions/dialex
```

### **Browser**

```html
<script src="https://cdn.jsdelivr.net/npm/@hyperlab-solutions/dialex/lib/dialex.min.js"></script>
```

## Python

```bash
pip install -U dialex
```

## Go

```bash
go get https://github.com/HyperLab-Solutions-Sdn-Bhd/dialex-sdk-go/dialex
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

## Go

```go
import "https://github.com/HyperLab-Solutions-Sdn-Bhd/dialex-sdk-go/dialex"

dial := dialex.New("apikey")
```



