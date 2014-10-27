# Documentation for scrollr v1.0.0 [+changelog](CHANGELOG.md)

If you have any problems, looking for some specific solutions or have a suggestion, please visit the [wiki knowledge base](https://github.com/mediastuttgart/scrollr-docs/wiki) or open a [ticket](https://github.com/mediastuttgart/scrollr-docs/issues)

## Quickstart

### Include files

Upload the `scrollr.min.css` and `scrollr.min.js` folder to your server and add the required files in the head section of your page.

```html
<!-- scrollr stylesheet -->
<link rel="stylesheet" href="your_assets_path/scrollr.min.css">

<!-- scrollr javascript -->
<script src="your_assets_path/scrollr.min.js"></script>
```

### IE Compatibility mode

To make scollr work with Internet Explorer 8+, be sure you're using the latest rendering mode for IE by adding the following meta tag in the head section of your page.

```html
<meta http-equiv="X-UA-Compatible" content="IE=edge">
```

### Add scrollr markup

Add the scrollr HTML code to the body section of your page. By default all required markup will be generated by scrollr. The type of the tag doesn't matter, it can be an article, a section or just a div, whatever.

```html
<div class="content">
  <p>... Content ...</p>
</div>
```

### Initialize scrollr

As scrollr is completely written without any dependencies, you can initialize scrollr in different ways

#### Basic Initialization

```javascript
var myElement = document.querySelector('.content');
var myScrollr = scrollr(myElement);
```

#### Initialize using the new operator

```javascript
var myElement = document.querySelector('.content');
var myScrollr = new scrollr(myElement);
```

#### Initialize as a jQuery plugin (jQuery required)

```javascript
var myScrollr = $(myElement).scrollr();
```
