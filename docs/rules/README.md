## Cases
### case 1
```
0-9:0-9 # case 1
```

### case 2
```
a-z0-9:a-z0-9 # case 2
```

### case 3
```
# case 3: symbol for comment is '#'
```

### case 4
```
'0-9': '0-9' # case 4
```

### case 5
```
'a-z0-9':'a-z0-9' # case 5
```

### case 6
```
"a-z0-9":"a-z0-9" # case 6
```

### case 7
```
"A-Z0-9":"A-Z0-9" # case 7
```

### case 8
```
'A-Z0-9':'A-Z0-9' # case 8
```

### case 9
```
"a-zA-Z0-9":"a-zA-Z0-9" # case 9 
```

### case 10
```
'a-zA-Z0-9':'a-zA-Z0-9' # case 10 
```

### case 11
```
# case 11: symbol for value can be '' or "" or value:value
```

### case 12
```
start-value:end-value # case 12
```

### case 13
```
'start-hash-type':'end-hash-type' # case 13, example: 'SHA-256:SHA-256', 'MD5:SHA-256', 'SHA-384:SHA-384' etc
```

### case 14
```
"start-hash-type":"end-hash-type" # case 14, example: "SHA-256:SHA-256", "MD5:SHA-256", "SHA-384:SHA-384" etc
```

## Rules: Input, Output
- `a-zA-Z0-9`: regex just means that any lower case alphabet character from "a to z" is acceptable, as well as capital letters "A to Z" and the numbers "0 to 9" with "" or '' or without this "" and ''
- `/\d+/g` or `[^0-9]`: regex that return just numbers with "" or '' or without this "" and ''
- `a-z`: regex just means that any lower case alphabet character from "a to z" is acceptable with "" or '' or without this "" and ''
- `A-Z`: regex just means that any capital case alphabet character from "A to Z" is acceptable with "" or '' or without this "" and ''
- `hash-type:hash-type`: as SHA-256:SHA-256, MD5:SHA-256, SHA-384:SHA-384 etc with "" or '' or without this "" and ''
- `"hash-type":"hash-type"`: "SHA-256:SHA-256", "MD5:SHA-256", "SHA-384:SHA-384" etc with ""
- `'hash-type':'hash-type'`: 'SHA-256:SHA-256', 'MD5:SHA-256', 'SHA-384:SHA-384' etc with ''
- `'hash':'hash-type'`: 'MD5:SHA-256', 'MD5:SHA-384' etc with ""
- `'hash-type':'hash'`: 'SHA-256:MD5', 'SHA-384:MD5' etc with ""
- `"hash":"hash-type"`: "MD5:SHA-256", "MD5:SHA-384" etc with ""
- `"hash-type":'hash"`: "SHA-256:MD5", "SHA-384:MD5" etc with ""
