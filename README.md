# ie8.js
Polyfill for JavaScript methods absent in Internet Explorer 8. Around 2KB gzipped.

## License
The polyfill source code comes from [Mozilla Developer Network](https://developer.mozilla.org/en-US/docs/MDN/About), which are in public domain, therefore this compilation is also released into public domain under [CC0 Public Domain Dedication](LICENSE).

## Usage
Put this in your HTML.
```html
<!--[if lt IE 9]>
  <script src="ie8.min.js"></script>
<![endif]-->
```

## What’s Inside

Below is a list of things included in this polyfill.

           Name              |      Absent in      
-----------------------------|:----------------------:
Object.create                | Internet Explorer 7, 8
Object.defineProperties      | Internet Explorer 7, 8
Object.keys                  | Internet Explorer 7, 8
Date.prototype.toISOString   | Internet Explorer 7, 8
Date.now                     | Internet Explorer 7, 8
Array.isArray                | Internet Explorer 7, 8
JSON                         | Internet Explorer 7
Function.prototype.bind      | Internet Explorer 7, 8
String.prototype.trim        | Internet Explorer 7, 8
Array.prototype.indexOf      | Internet Explorer 7, 8
Array.prototype.lastIndexOf  | Internet Explorer 7, 8
Array.prototype.every        | Internet Explorer 7, 8
Array.prototype.some         | Internet Explorer 7, 8
Array.prototype.forEach      | Internet Explorer 7, 8
Array.prototype.map          | Internet Explorer 7, 8
Array.prototype.filter       | Internet Explorer 7, 8
Array.prototype.reduce       | Internet Explorer 7, 8
Array.prototype.reduceRight  | Internet Explorer 7, 8

## Unpolyfillable

And below is a list of things that I failed to find a way to implement a polyfill. If you can fix any of this, please send a pull request.

           Name                 |      Absent in     
--------------------------------|:-----------------------:
Object.defineProperty           | Internet Explorer 7
Object.seal                     | Internet Explorer 7, 8
Object.freeze                   | Internet Explorer 7, 8
Object.preventExtensions        | Internet Explorer 7, 8
Object.isSealed                 | Internet Explorer 7, 8
Object.isFrozen                 | Internet Explorer 7, 8
Object.isExtensible             | Internet Explorer 7, 8
Object.getOwnPropertyDescriptor | Internet Explorer 7
Object.getOwnPropertyNames      | Internet Explorer 7, 8
