# JavaScript 30

This is my fork of [Wes Bos' JS30 Course](https://javascript30.com).

I want to document what I learn throughout the process here.

## Drum Kit

1. Data Attributes are useful for custom attributes on HTML elements when other attributes aren't right. You specify them as `data-<name>` and can use CSS/JS selectors on them.
2. You can interpolate values into selectors.
3. Audio has a method called `currentTime` which you can set to 0 to restart the audio. It also has a `play()` method.
4. 'transitionend' is an event.
5. All keys have a specific event keycode. See [keycode.info](http://keycode.info).

## Clock

1. Chrome DevTools has a little thing you can click to adjust your `transition-timing-function` curve.
2. `setInterval()` is provided two parameters. The first is the function/expression. The second is the specified interval in milliseconds. It calls the function/expression every specified interval.
3. Things have origins that you can transform.

## CSS Variables

1. CSS' variables can be updated with JS.
2. CSS uses `--` for variable declaration. You specify `var(--variable)` for usage.
3. CSS variables must be attached to an element, of which `:root` is the highest.
4. The `filter` CSS property applies graphical effects to an element.
5. `change` is an event.
6. The `dataset` method can be used on an element to list all the data-attributes of an element.
7. You can select CSS variables by using the `document` element, accessing `documentElement` which is the root element, accessing style, then setting the property of the CSS variable (`--variableName`).

## Array Cardio Day

1. The `filter` method iterates over an array and returns each element that returns true within the function.
```javascript
const result = arrayExample.filter(function(arrayElement) {
  return true; // All elements of the array will be returned into the result array.
});
```
2. The `sort` method compares each element of the array. You pass it a function that returns 1 or -1, which will correspond to how things get sorted.
3. `console.table` exists.
4. The `reduce` method condenses an array to one value.
5. The `map` method takes an array, does something to each element, then returns a new array with the modified elements, with the original array unchanged.
6. There are two ways to convert a NodeList to an Array. You can use a spread, `[...elements]`, which takes all the elements out of something and put them into an array. Or you can use `Array.from(elements)`.
