This is a new [**React Native**](https://reactnative.dev) project, bootstrapped using [`@react-native-community/cli`](https://github.com/react-native-community/cli).


## Step 1: Start the project

Run `npx react-native run-android` within the project and observe the results within the Metro.

## Step 2: Observe the issue

Within the Metro you will notice that when you touch move, the log will print a message with a counter. This counter resets when touch ends. The issue occurs when dragging is recognized by native recognizer within scroll view and touch move event is replaced with dragging event and scroll is happening. Then the touch is cancelled and we are not getting the touch end event. We can trigger touch cancelled event, but I still need to see all touch move events which are happening during drag.



