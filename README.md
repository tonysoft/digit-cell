[Published on NPM](https://www.npmjs.com/package/digit-cell)


## &lt;digit-cell&gt;

The `digit-cell` element displays an icon. By default an icon renders as a 24px
square.

See: [Demo](https://tonysoft.github.io/digit-cell).

## Usage

### Installation

```
npm install --save @polymer/iron-icon
```

### In an HTML file

```html
<html>
  <head>
    <script type="module">
      import '@polymer/iron-icon/iron-icon.js';
    </script>
  </head>
  <body>
    <iron-icon src="demo/location.png"></iron-icon>

    <!-- You can use an icon from an imported iconset. -->
    <script type="module">
      import '@polymer/iron-icons/iron-icons.js';
    </script>
    <iron-icon icon="search"></iron-icon>
  </body>
</html>
```

### In a Polymer 3 element

```js
import {PolymerElement} from '@polymer/polymer/polymer-element.js';
import {html} from '@polymer/polymer/lib/utils/html-tag.js';

import '@polymer/iron-icon/iron-icon.js';

class ExampleElement extends PolymerElement {
  static get template() {
    return html`
      <iron-icon src="demo/location.png"></iron-icon>
    `;
  }
}

customElements.define('example-element', ExampleElement);
```

## Contributing

If you want to send a PR to this element, here are the instructions for running
the tests and demo locally:

### Installation

```sh
git clone https://github.com/PolymerElements/iron-icon
cd iron-icon
npm install
npm install -g polymer-cli
```

### Running the demo locally

```sh
polymer serve --npm
open http://127.0.0.1:<port>/demo/
```

### Running the tests

```sh
polymer test --npm
```
