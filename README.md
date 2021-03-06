<div align="center">
<h1>mb</h1>
<img height="80" width="80" alt="goat" src="https://d1j8pt39hxlh3d.cloudfront.net/development/emojione/4.0/833/14168.svg?1533081835" />

Exception-free nested nullable attribute accessor.
An alternative to [facebookincubator/idx](https://github.com/facebookincubator/idx) in 57 bytes.
</div/>

<hr />

## Install
Just copy/paste this function into your project:
``` javascript
var mb=(f,...p)=>(o,i=o[f])=>i&&p[0]!=null?mb(...p)(i):i
```
Alternatively, you can download [mb.js](https://raw.githubusercontent.com/burakcan/mb/master/mb.js).

## Use
``` javascript
var getHello = mb('a', 'b', 0, 'hello');

var obj1 = {
  a: {
    b: [{ hello: 'world' }]
  }
};

var obj2 = {
  c: {
    d: 'e'
  }
};

getHello(obj1); // world
getHello(obj2); // undefined
```

## Contribution and Code-Golfing

1. Clone and shorten current code.
2. Please open `test.html` in your browser and open console to see if all the tests pass.

## Contributors
- [Fatih Kadir Akin](https://github.com/f)
- [Burak Can](https://github.com/burakcan)
- [Eser Ozvataf](https://github.com/eserozvataf)
