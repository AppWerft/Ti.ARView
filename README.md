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
  backgroundColor : 'transparent'
});
// adding all POIs as view
for (var i=0;i<10;i++) {
  arContainer.add(Ti.UI.createLabel({
    text : i,
    center : {
      x : i/10*100 + '%',
      y : '50%'
    }
  }))

}

arContainer.start();
// now the contentContainer followes the heading of compass 
```

Attention: if you enable trueHeading you need location permission!
