## Customizable material switch for react-native
<p align="center">
    <img src ="http://oi57.tinypic.com/2rysl94.jpg" />
</p>

### Content
- [Installation](#installation)
- [Usage example](#usage-example)
- [Properties](#properties)
- [Events](#events)
- [Live example](#live-example)
- [Questions?](#questions)

### Installation
```bash
npm install react-native-base-switch
```

### Usage example
```javascript
import React, { Component } from "react";
import { Switch }  from 'react-native-base-switch';

class Application extends Component {
  onChangeState(isActive) {
    console.log(isActive)
  }
  
  render() {
    return (
      <View>
        <Switch onChangeState={this.onChangeState}/>
      </View>
    );
  }
}
```

### Properties
* `active` (Boolean) - Initial switch state (default: false),
* `style` (Object) - Styles for outer container (margins, ...),
* `padding` (Integer) - Padding of outer container (default: 2),
* `inactiveButtonColor` (String) - Button color  (default: '#2196F3'),
* `inactiveButtonPressedColor` (String) (default: '#42A5F5'),
* `activeButtonColor` (String) (default: '#FAFAFA'),
* `activeButtonPressedColor` (String) (default: '#F5F5F5'),
* `buttonShadow` (Object) - Shadow style for button (default: { shadowColor: '#000', shadowOpacity: 0.5, shadowRadius: 1, shadowOffset: { height: 1, width: 0 }},
* `activeBackgroundColor` (String) - (default: 'rgba(255,255,255,.5)'),
* `inactiveBackgroundColor` (String) - (default: 'rgba(0,0,0,.5)'),
* `buttonRadius` (Number) - (default: 15),
* `switchWidth` (Number) - (default: 40),
* `switchHeight` (Number) - (default: 20),
* `buttonContent` (React.Component) - Custom inline content for switch button (default: null),
* `enableSlide` (Boolean) - (default: true),
* `switchAnimationTime` (Number) - Switch animation duration (default: 200),
* `borderWidth` (Number) ,
* `borderColor` (Number) ,

### Events
* `onActivate`: This function is called when the switch is activated.
* `onDeactivate`: This function is called when the switch is deactivated.
* `onChangeState`: Sends the current state of switch.

### Live example
```sh
git clone git@github.com:Recr0ns/react-native-material-switch.git
cd react-native-material-switch/examples
npm install
open ios/switchExample.xcodeproj
```
Then `Cmd+R` to start the React Packager, build and run the project in the simulator.

### License
MIT License
This module base on https://github.com/recr0ns/react-native-material-switch . Thank @recr0ns.
### Questions?
Feel free to [create an issue](https://github.com/tiempham/react-native-base-switch.git/issues)
