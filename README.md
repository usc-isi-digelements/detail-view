# detail-view

A Polymer Element showing details, extractions, images, and/or a button link.

### Example
```js
details = [{
  name: 'Description',
  text: 'This is a list of my favorite software projects!'
}];

extractions = [{
  name: 'Favorite Projects',
  data: [{
    confidence: 'high',
    highlight: true,
    icon: 'search',
    link: 'https://github.com/DigElements',
    styleClass: 'extraction',
    text: 'DigElements'
  }]
}];

images = [{
  link: 'https://github.com/DigElements',
  source: 'dig.png'
}];
```

```html
<detail-view
  button-link="https://google.com"
  button-text="Open"
  details="[[details]]"
  extractions="[[extractions]]"
  images="[[images]]">
</detail-view>
```

### Styling

`<detail-view>` provides the following custom properties and mixins for styling:

Custom property                        | Description                                 | Default
---------------------------------------|---------------------------------------------|-----------------------
`--detail-view-high-confidence-color`  | The color of the high confidence icon.      | none
`--detail-view-highlighted-text-color` | The color of the highlighted text.          | none
`--detail-view-hover-color`            | The color of the extraction label on hover. | --secondary-text-color
`--detail-view-label-color`            | The color of the extraction label.          | --primary-text-color
`--detail-view-label-mixin`            | Mixin applied to the extraction label.      | {}
`--detail-view-low-confidence-color`   | The color of the low confidence icon.       | none
`--detail-view-title-color`            | The color of the extraction title.          | --secondary-text-color

### Dependencies

Dependencies are installed using [Bower](http://bower.io/):

    npm install -g bower
    bower install

### Testing

Tests are run using [web-component-tester](https://github.com/Polymer/web-component-tester):

    npm install -g web-component-tester
    wct

### Demonstration & Documentation

Demonstration and documentation are viewed using [polyserve](https://github.com/PolymerLabs/polyserve):

    npm install -g polyserve
    polyserve

