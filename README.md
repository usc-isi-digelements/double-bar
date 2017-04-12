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

