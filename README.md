[meme-maker](https://dirkarnez.github.io/meme-maker)
====================================================
### TODOs
- [ ] decoupling canvas, by using [dirkarnez/image-js-playground](https://github.com/dirkarnez/image-js-playground)
### Using
- [fabricjs/fabric.js: Javascript Canvas Library, SVG-to-Canvas (& canvas-to-SVG) Parser](https://github.com/fabricjs/fabric.js)
  - Examples
    - http://fabricjs.com/loadfonts
    - http://fabricjs.com/kitchensink
    - http://fabricjs.com/touch-events
    - http://fabricjs.com/clipping
    - http://fabricjs.com/dynamic-patterns
    - http://fabricjs.com/bounding-rectangle
    - http://fabricjs.com/image-filters
    - http://fabricjs.com/opacity_mouse_move
    - **https://devpost.com/software/built-with/fabric-js**
- https://github.com/wanadev/perspective.js/blob/master/demo/demo.html

### Snippets
```js
const canvas = document.getElementById("canvas");
const ctx = canvas.getContext("2d");
const arr = new Uint8ClampedArray(40_000);

// Fill the array with the same RGBA values
for (let i = 0; i < arr.length; i += 4) {
  arr[i + 0] = 0; // R value
  arr[i + 1] = 190; // G value
  arr[i + 2] = 0; // B value
  arr[i + 3] = 255; // A value
}

// Initialize a new ImageData object
let imageData = new ImageData(arr, 200);

// Draw image data to the canvas
ctx.putImageData(imageData, 20, 20);
```
### Reference
- [HTML5 Canvas Export to High Quality Image Tutorial | Konva - JavaScript 2d canvas library](https://konvajs.org/docs/data_and_serialization/High-Quality-Export.html)
- [How to resize text on canvas? | Konva - JavaScript 2d canvas library](https://konvajs.org/docs/select_and_transform/Resize_Text.html)
