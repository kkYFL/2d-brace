# brace

[原始仓库]https://github.com/thlorenz/brace.git

[业务改造仓库]https://github.com/kkYFL/2d-brace.git

## Installation

    npm install brace

## Example

```js
var ace = require('brace');
require('brace/mode/javascript');
require('brace/theme/monokai');

var editor = ace.edit('javascript-editor');
editor.getSession().setMode('ace/mode/javascript');
editor.setTheme('ace/theme/monokai');
```

Include the above as an **entry** in your browserify build, add a `<div id="javascript-editor"></div>` to your html page and
a JavaScript editor will appear.

This editor will show error/warning annotations if your browser supports WebWorkers
created via a blob URL (see testling support badge on top).

Please consult the [detailed example](https://github.com/thlorenz/brace/tree/master/example) for more information.


## Can I use it with TypeScript?

Yes, brace includes modular type definitions so you can do normal import statements and type safety checking
with TypeScript. The example above becomes:

```ts
import * as ace from 'brace';
import 'brace/mode/javascript';
import 'brace/theme/monokai';

const editor = ace.edit('javascript-editor');
editor.getSession().setMode('ace/mode/javascript');
editor.setTheme('ace/theme/monokai');
```

## Test

    npm explore brace
    npm test

## 分支
2d-branch 业务改造分支

