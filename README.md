### pica
---
https://github.com/nodeca/pica

```js
import Pica from 'pica';
const pica = Pica();
pica.resize(img, canvas).then(...);

const pica = require('pica')();
pica.resize(from, to, {
  unsharpAmount: 80,
  unsharpRadius: 0.6,
  unsharpThreshold: 2
})
.then(result => console.log('resize done!'));

pica.resize(from, to)
  .then(result => pica.toBlob(result, 'image/jpeg', 0.90))
  .then(blob => console.log('resized to canvas & created blob!'));

const pica = require('pica')({ features: [ 'js', 'wasm', 'ww', 'cib' ]});
```

```
npm install pica
npm install babelify @babel/core @babel/preset-env
bower install pica
```

```
{
  resolve: {
    alias: {
      pica: 'pica/dist/pica.js',
    },
  }
}
```


