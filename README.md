### jsoneditor
---
https://github.com/josdejong/jsoneditor

```
npm install jsoneditor
bower install jsoneditor

npm install
npm run build
npm run watch

npm install
browserify ./index.js -o ./jsoneditor.custom.js -s JSONEditor
browserify ./index.js -o ./jsoneditor.custom.js -s JSONEditor -x brace-x brace/mode/json -x brace/ext/searchbox
uflifyjs ./jsoneditor.custom.js -o ./jsoneditor.custom.min.js -m -c
```

```js
var container = document.getElementById("jsoneditor");
var options = {};
var editor = new JSONEditor(container, options);

var json = {
  "Array": [1, 2, 3],
  "Boolean": true,
  "Null": null,
  "Number": 123,
  "Object": {"a": "b", "c": "d"},
  "": ""
};
editor.set(json);

var json = editor.get();
```

```
```


