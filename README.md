# bpmn-moddle-auto-layout


Get a layouted diagram of a bpmn-process without graphical representation.

__bpmn-moddle-auto-layout__  is built on top of [bpmn-moddle](https://github.com/bpmn-io/bpmn-moddle).


## Usage

__Preconditions:__ The diagram has to have __exactly one single startevent__. Up to now, elements with children are not supported.

```javascript
var AutoLayout = require('./index');

var xmlWithoutDi = '<?xml version="1.0" encoding="UTF-8"?>' +
                      '<bpmn:definitions>' +
                          /*
                          see example.js for closer look at the
                          passed in xml
                          */
                      '</bpmn:definitions>';

var autoLayout = new AutoLayout();



autoLayout.layoutProcess(xmlWithoutDi,function(err,xml){
  console.log(xml)
});
```


## Resources

*   [Issues](https://github.com/bpmn-io/bpmn-moddle-auto-layout/issues)


## License

Use under the terms of the [MIT license](http://opensource.org/licenses/MIT).
