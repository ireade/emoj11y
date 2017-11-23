# \<emoj11y-element\>

[![Published on webcomponents.org](https://img.shields.io/badge/webcomponents.org-published-blue.svg)](https://www.webcomponents.org/element/ireade/emoj11y)

An accessible emoji component

## Demo

<!--
```
<custom-element-demo></custom-element-demo>
  <template>
    <style>
      emoj11y-element {
        margin-top: 20px;
        font-size: 20px;
      }
    </style>
    <link rel="import" href="emoj11y-element.html">
    <next-code-block></next-code-block>
  </template>
</custom-element-demo>
```
-->
```html
<emoj11y-element shortname="smile"></emoj11y-element>
<emoj11y-element shortname="dizzy_face" label="I'm so Dizzy"></emoj11y-element>
<emoj11y-element shortname="dancer" skin-tone="4"></emoj11y-element>
```

## Usage

1. Install with Bower

```
mkdir emoj11y-demo && cd emoj11y-demo
bower install emoj11y-element
```

2. Include the element on a page

```
<!doctype html>
<html>
  <head>
    <meta charset="utf-8">
    <title>Emoj11y Demo</title>
    <script src="bower_components/webcomponentsjs/webcomponents-lite.js"></script>
    <link rel="import" href="bower_components/emoj11y/emoj11y-element.html">
  </head>
  <body>
    <emoj11y-element shortname="dancer" skin-tone="4"></emoj11y-element>
  </body>
</html>
```

### Options

These are the available options you can specify

Option | Description
-------|------------
`shortname` (required) | The shortname for the element. Must be a valid [emojione shortname](https://www.emojione.com/emoji/v3)
`label` | An alternate label for the emoji. Defaults to the shortname
`skinTone` | A number from 1-6 representing the skin tone of the emoji (if applicable)

## Contributing

### Install the Polymer-CLI

First, make sure you have the [Polymer CLI](https://www.npmjs.com/package/polymer-cli) installed. Then run `polymer serve` to serve your element locally.

### Viewing Your Element

```
$ polymer serve
```

### Running Tests

```
$ polymer test
```

Your application is already set up to be tested via [web-component-tester](https://github.com/Polymer/web-component-tester). Run `polymer test` to run your application's test suite locally.
