# Demo of generating a skills wheel

Check it out at: https://inclusiveclassrooms.github.io/wheel-demo/

The function to generate the wheel can be downloaded to a `wheel.js` file with:

```bash
curl https://cdn.rawgit.com/InclusiveClassrooms/wheel-demo/7dba2c68/wheel.js > wheel.js
```

The function will generate a "skills wheel" inside of an element you specify at a position you specify:

Typical use:

#### Arg #1: Array of 36 objects, each object should have keys of: `question` and `answer`

#### Arg #2: Element to insert the wheel into, examples are:

`'#wheel-container'`, `'.wheel1'`, etc

#### Arg #3: Object representing the dimentions of the wheel.

The object should have keys of `centre`, `height` and `width`

#### Example use:

```js
drawWheel(arr, '#wheel-container', {centre: 250, height: 500, width: 500})
```
