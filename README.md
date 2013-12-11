# jquery-sharer

Social share buttons plugin for jQuery

## Installation

Include stylesheet in your document's `<head>`

    <link rel="stylesheet" src="jquery.sharer.css">

Include script after jQuery library

    <script src="jquery.sharer.js"></script>

## Usage

Add a container element

    <div id="sharer-container"></div>

Initialise

    <script type="text/javascript">$("#sharer-container").sharer()</script>

## Options

### networks

An array containing enabled networks

    "networks": ["facebook", "twitter", "linkedin", "tumblr", "googleplus", "reddit", "pinterest", "stumbleupon", "taringa"]

### template

Base object for buttons

    "template":  $(<a class="sharer-icon" />)

### class

Class added to buttons

    "class": "sharer-icon-%network.id%"

### label

Button title

    "label": "Share on %network.name%"

### title

Share title. Defaults to current title

    "title": null


### description

Share description. Defaults to document's meta description

    "description": null

### url

Share URL. Defaults to current location

    "url": null