# jquery-sharer

Social share buttons plugin for jQuery, supports Facebook, Twitter, LinkedIn, Tumblr, Google+, reddit, Pinterest, StumbleUpon and Taringa!

## Installation

Include stylesheet in your document's `<head>`

```html
<link rel="stylesheet" src="jquery.sharer.css">
```

Include script after jQuery library

```html
<script src="jquery.sharer.js"></script>
```

## Usage

Add a container element

```html
<div id="sharer-container"></div>
```

Initialise

```html
<script type="text/javascript">$("#sharer-container").sharer()</script>
```

## Options

### networks

An array containing enabled networks

```javascript
"networks": ["facebook", "twitter", "linkedin", "tumblr", "googleplus", "reddit", "pinterest", "stumbleupon", "taringa"]
```

### template

Base object for buttons

```javascript
"template":  $('<a class="sharer-icon" />')
```

### class

Class added to buttons

```javascript
"class": "sharer-icon-%network.id%"
```

### label

Button title

```javascript
"label": "Share on %network.name%"
```

### title

Share title. Defaults to current title

```javascript
"title": null
```


### description

Share description. Defaults to document's meta description

```javascript
"description": null
```

### url

Share URL. Defaults to current location

```javascript
"url": null
```

## Networks

Add, or modify, a network using `$.sharer.networks` object

```javascript
$.sharer.networks["yet-another-social-network"] = {
    "name": "Yet Another Social Network",
    "url": "http://www.yetanothersocialnetwork.com/share?url=%url%" // also %title% and %description% are available
};
```

## Overriding global defaults

Override global defaults using `$.sharer.options` object

```javascript
$.sharer.options["label"] = "Compartir en %network.id%";
```

## Demo

http://marcojetson.github.io/jquery-sharer/

## Credits

- Minimal Social Media Icons by [softarea](http://www.softarea.in)
- Heavily inspired in [jquery-share](https://github.com/iatek/jquery-share)