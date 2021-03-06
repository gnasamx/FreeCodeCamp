:coffee:

Just like people inherit genes from their parents, an object inherits its `prototype` directly from the constructor function that created it. For example, here the Bird constructor creates the duck object:

```js
function Bird(name) {
  this.name = name;
}

let duck = new Bird("Donald");
```

`duck` inherits its `prototype` from the `Bird` constructor function. You can show this relationship with the `isPrototypeOf` method:

```js
Bird.prototype.isPrototypeOf(duck);
// returns true
```

:fire:

Use `isPrototypeOf` to check the prototype of `beagle`.
