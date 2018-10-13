# Ti.ARView

Module for Axways Titanium for ARView

## Usage

```javascript
const ArView = require("ti.arview");
const WIDTH = 5000;

var arContainer = ArView.createView({
  width : WIDTH,
  height : Ti.UI.FILL,
  trueHeading : false,
  offset : 0,
  autostart : true
});
// adding all POIs as view
// this example shows degrees:
for (var i=0; i<36; i++) {
  arContainer.add(Ti.UI.createLabel({
    text : i + '0°',
    center : {
      x : i/10*100 + '%',
      y : '50%'
    }
  }))
};

arContainer.start();
// now the contentContainer followes the heading of compass 
```

Attention: if you enable trueHeading you need location permission!
