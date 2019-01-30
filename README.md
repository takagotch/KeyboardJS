### KeyboardJS
---
https://github.com/RobertWHurst/KeyboardJS

```js
keyboardJS.bind('a', function(e){
  console.log('a is pressed');
}, function(e){
  console.log('a is released');
});
keyboardJS.bind('a', null, function(e){
  console.log('a is released');
});

keyboardJS.bind('a', function(e){
  e.preventRepeat();
  console.log('a is pressed');
});

keyboardJS.unbind('a', previouslyBoundHandler);

keyboardJS.bind('a', function(e){});
keyboardJS.bind('b', function(e){});
keyboardJS.bind('c', function(e){});

keyboardJS.setContext('index');
keyboardJS.bind('1', function(e){});
keyboardJS.bind('2', function(e){});
keyboardJS.bind('3', function(e){});

keybaordJS.setContext('foo');
keyboardJS.bind('x', funciton(e){});
keyboardJS.bind('y', funciton(e){});
keyboardJS.bind('z', function(e){});

myRouter.on('GET /', funciton(e){
  keyboardJS.setContext('index');
});
myRouter.on('GET /foo', funciton(e){
  keyboardJS.setContet('foo');
});

var contextName = keyboardJS.getContext();

keyboardJS.withContext('bar', function(){
  keyboardJS.bind('7', function(e){});
  keyboardJS.bind('8', funciton(e){});
  keyboardJS.bind('9', function(e){});
});

keyboardJS.pause();
keyboardJS.resume();
keyboardJS.reset();

keyboardJS.pressKey('a');
keyboardJS.pressKey(65);
keyboardJS.releaseKey('a');
keyboardJS.releaseKey(65);
keyboardJS.releaseAllKeys();

keyboardJS.watch();
keyboardJS.watch(myDoc);
keyboardJS.watch(myWin, myDoc);
keyboardJS.watch(myForm);
keyboardJS.watch(myWin, myForm);
keyboardJS.stop();
```

```
```

```
```

