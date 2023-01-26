```

0-9:0-9 # case 1
a-z0-9:a-z0-9 # case 2

# case 3: symbol for comment is '#'

'0-9': '0-9' # case 4

'a-z0-9':'a-z0-9' # case 5
"a-z0-9":"a-z0-9" # case 6

"A-Z0-9":"A-Z0-9" # case 7
'A-Z0-9':'A-Z0-9' # case 8

"a-zA-Z0-9":"a-zA-Z0-9" # case 9 
'a-zA-Z0-9':'a-zA-Z0-9' # case 10 

# case 11: symbol for value can be '' or "" or value:value

start-value:end-value # case 12
'start-hash-type':'end-hash-type' # case 13, example: 'SHA-256:SHA-256', 'MD5:SHA-256', 'SHA-384:SHA-384' etc

"start-hash-type":"end-hash-type" # case 14, example: "SHA-256:SHA-256", "MD5:SHA-256", "SHA-384:SHA-384" etc
```
