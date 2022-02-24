## @labdao/openlab-applayer-client

OpenLab application layer REST API client.

> !! NOTE: under active development, please wait until the first release to use this package

### Compatibility

The module should work in the following environments:

Environment
* Node.js
* Webpack
* Browserify

Language level
* ES5 - you must have a Promises/A+ library installed
* ES6

Module system
* CommonJS
* ES6 module system

It can be used in both TypeScript and JavaScript. In TypeScript, the definition should be automatically resolved via `package.json`. ([Reference](http://www.typescriptlang.org/docs/handbook/typings-for-npm-packages.html))

### Installation

navigate to the folder of your consuming project and run one of the following commands.

_published:_

```
npm install @labdao/openlab-applayer-client@0.0.1 --save
```

_unPublished (not recommended):_

```
npm install PATH_TO_GENERATED_PACKAGE --save

### Usage

```js
const { OpenLabApi } = require('@labdao/openlab-applayer-client')

const api = new OpenLabApi({ baseUrl: 'your_baseurl_here' })

api.apps().then(r => console.log(r.data))

api.app('alphafold').then(r => console.log(r.data)))

api.jobStatus(
  appname='alphafold',
  jobid='73222306-cd7c-4e71-bd82-9e4f6123976c'
).then(r => console.log(r.data))
```

### License

MIT licensed