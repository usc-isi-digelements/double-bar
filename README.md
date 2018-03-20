# double-bar

A Polymer Element showing two horizontal-bar elements.  The left horizontal-bar is built using given properties.  The right horizontal-bar is built using the results of an elasticsearch query and shows the total count of documents in the elasticsearch index minus the given count (shown in the left bar).

### Example
```html
<double-bar
  client="[[client]]"
  index-name="[[indexName]]"
  index-types="[[indexTypes]]"
  query-field="[[queryField]]"
  count="10"
  item-id="abc123"
  max="20"
  text="The Bar"
  selected="{{selected}}"
  other-count="{{otherCount}}"
  max-other-count="{{maxOtherCount}}">
</double-bar>
```

### Styling

`<double-bar>` provides the following custom properties and mixins for styling:

Custom property                        | Description                                              | Default
---------------------------------------|----------------------------------------------------------|--------
`--double-bar-left-color`              | The color of the left bar.                               | --paper-grey-300
`--double-bar-left-count-color`        | The color of the left count label.                       | --paper-grey-900
`--double-bar-left-height`             | The height of the left bar.                              | 20px
`--double-bar-left-title-color`        | The color of the left title label.                       | --paper-grey-900
`--double-bar-left-title-hover-color`  | The color of the left title label on hover (if a link).  | --paper-indigo-900
`--double-bar-right-color`             | The color of the right bar.                              | --paper-grey-300
`--double-bar-right-count-color`       | The color of the right count label.                      | --paper-grey-900
`--double-bar-right-height`            | The height of the right bar.                             | 20px
`--double-bar-right-title-color`       | The color of the right title label.                      | --paper-grey-900
`--double-bar-right-title-hover-color` | The color of the right title label on hover (if a link). | --paper-indigo-900

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

