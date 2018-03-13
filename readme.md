# node-sass test for issue sass/node-sass#2287

## Failing test

```
  npm install node-sass@4.8.2
  npm test
```

Result:

```
{
  "status": 1,
  "file": "C:/Users/vhkrausser/teste-sass/index.scss",
  "line": 1,
  "column": 1,
  "message": "File to import not found or unreadable: var.scss.\nParent style sheet: C:/Users/vhkrausser/teste-sass/index.scss",
  "formatted": "Error: File to import not found or unreadable: var.scss.\n       Parent style sheet: C:/Users/vhkrausser/teste-sass/index.scss\n        on line 1 of index.scss\n>> @import 'var.scss';\n\n   ^\n"
}
```

## Working scenario

```
  npm install node-sass@4.7.2
  npm test
```

Result:

```
.test {
  background-color: #000; }
```