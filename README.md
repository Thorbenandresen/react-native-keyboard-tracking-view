# react-native-keyboard-tracking-view
A react native UI component that enables “keyboard tracking" for this view and it's sub-views. Would typically be used when you have a TextInput inside this view.

## Installation

- Install using `npm`:

	```
	npm i react-native-keyboard-tracking-view --save
	```

- Locate the module lib folder in your node modules:
	`PROJECT_DIR/node_modules/react-native-keyboard-tracking-view/lib`.

- Drag the `KeyboardTrackingView.xcodeproj` project file into your project

![](https://github.com/wix/react-native-keyboard-tracking-view/blob/master/img/add_proj.png)

- Add `libTrackingView.a` to your target's **Linked Frameworks and Libraries**.

![](https://github.com/wix/react-native-keyboard-tracking-view/blob/master/img/add_proj.png)

## How To Use
Require the native component:

```js
import React, {
  requireNativeComponent
} from 'react-native';

const KeyboardTrackingView = requireNativeComponent('KeyboardTrackingView', null);
```

Now use it in your jsx as the parent of the views you whish to track the keyboard (usually wraps a TextInput at the bottom of the screen):

```jsx
<KeyboardTrackingView style={styles.textInputContainer}>
	<TextInput style={styles.textInput} />
</KeyboardTrackingView>
```

## Example Project

Check out the full example project [here](https://github.com/wix/react-native-keyboard-tracking-view/tree/master/example).

In the example folder, perform `npm install` and then run it from the Xcode project.
