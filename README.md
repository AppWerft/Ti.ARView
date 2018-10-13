# Ti.ARView

Module for Axways Titanium for ARView

## Usage

```javascript
const ArView = require("ti.arview");

var arContainer = ArView.createView({
  width : 20000,
  height : Ti.UI.FILL,
  trueHeading : false,
  backgroundColor : 'transparent'
});
// adding all POIs as view
arContainer.start();
// now the contentContainer followes the heading of compass 
```

Attention: if you enable trueHeading you need location permission!
