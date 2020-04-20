# summernote-image-title
A plugin for the [Summernote](https://github.com/summernote/summernote/) WYSIWYG editor.

Adds a button to the image popover to edit title and alt attributes.

### Installation

#### 1. Include JS

This plugin is available on NPM or Bower:

```
npm install summernote-image-title --save
```

```
bower install summernote-image-title --save
```

Include the following code after Summernote:

```html
<script src="summernote-image-title.js"></script>
```

#### 2. Supported languages

Currently available in:
- English
- French
- Korean (thanks to [@lqez](https://github.com/lqez) and [@pincoin](https://github.com/pincoin))
- Portuguese (thanks to [@parg-programador](https://github.com/parg-programador))
- Spanish (thanks to Cristian from [Websfrits.com](http://www.websfrits.com/))
- Català (thanks to Cristian from [Websfrits.com](http://www.websfrits.com/))
- German (thanks to [@osworx](https://github.com/osworx))
- Russian (thanks to [@anton-z](https://github.com/anton-z))
- Dutch (thanks to [MysticEarth](https://github.com/MysticEarth))
- Thai (thanks to [@pincoin](https://github.com/pincoin))
- Japanese (thanks to [@cmonos](https://github.com/cmonos))
- Traditional Chinese (thanks to [@SuYiLun41](https://github.com/SuYiLun41))
- Arabic (thanks to [@abdulrahman19](https://github.com/abdulrahman19))
- Persian (thanks to [@kiaksarg](https://github.com/kiaksarg))
- Romanian (thanks to [@totpero](https://github.com/totpero))

Contributions are welcomed!

#### 3. Summernote options

Finally, customize the Summernote image popover.
You can choose if you want to edit the alt attribute specifically or not with the option `specificAltField`:

```javascript
$(document).ready(function() {
    $('#summernote').summernote({
        imageTitle: {
          specificAltField: true,
        },
        lang: 'fr-FR',
        popover: {
            image: [
                ['imagesize', ['imageSize100', 'imageSize50', 'imageSize25']],
                ['float', ['floatLeft', 'floatRight', 'floatNone']],
                ['remove', ['removeMedia']],
                ['custom', ['imageTitle']],
            ],
        },
    });
});
```

### Example

You can see working pens here:
- [Summernote 0.8.11 / Bootstrap 3.3.6](http://codepen.io/asiffermann/pen/EKvMMm)
- [Summernote 0.8.11 / Bootstrap 4.1.3](http://codepen.io/asiffermann/pen/XorJOB)
