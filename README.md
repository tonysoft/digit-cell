[Published on NPM](https://www.npmjs.com/package/digit-cell)


## &lt;digit-cell&gt;

The `digit-cell` element represents a single Digit within some component or application like a Digital Clock
square.

See: [Demo](https://tonysoft.github.io/digit-cell).

## Usage

### Installation

```
npm install --save digit-cell
```

### In an HTML file

```html
<html>
  <head>
    <script type="module">
      import 'digit-cell.js';
    </script>
  </head>
  <body>
    <digit-cell value="7" size="50"></digit-cell>
  </body>
</html>
```

### In a Polymer 3 element

```js
import {html, PolymerElement} from '@polymer/polymer/polymer-element.js';

import 'digit-cell.js';

class ExampleElement extends PolymerElement {
  static get template() {
    return html`
      <digit-cell value="7" size="50"></digit-cell>
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
polymer serve -o
```

### Running the tests

```sh
polymer test --npm
```
