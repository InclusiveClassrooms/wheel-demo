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

#### Arg #3: File path of the faces svgs. E.g. `'assets'` or `'../assets'`

#### Arg #4: Object representing the configuration of the wheel

The object should have the following keys:
* `centre` # where the centre of the wheel is
* `height` # the height & width of the box the wheel is in
* `ratio` # the size of the wheel as a ratio
* `unique_string`: # a unique string to differentiate each wheel, ensure this string is different for each wheel you are rendering on the same page

#### A

#### Example use:

```js
drawWheel(arr, '#wheel-container', '', {centre: 250, height: 500}, 1, 'first')
```
