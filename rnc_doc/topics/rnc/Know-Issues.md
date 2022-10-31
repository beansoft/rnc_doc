[//]: # (title: Know Issues)

## Sorry, no physical iOS devices found! #73 on XCode 13

[Sorry, no physical iOS devices found! #73](https://github.com/beansoft/react-native-console/issues/73)

After some googling I've found that the `instruments` command has been removed from Xcode 13.

I've found it's not possible to fix this issue as there is broken in react-native ` 0.70.0` too.
For me, by using https://docs.libimobiledevice.org/libimobiledevice/latest/ with their cli util,
I can read the device name:
```
brew install libimobiledevice
ideviceinfo -s
DeviceName: iPhoneXRBean
```
then if you're using command by React Native CLI,
by: `npx react-native run-ios --device`
or given a device name:
```
npx  react-native run-ios --device iPhoneXRBean
Then errors will be thrown by Facebook's tool:
info Found Xcode project "AwesomeProject.xcodeproj"
error Could not find a device named: "iPhoneXRBean". Available devices:
  - MyMac (F5256792-DDDD-DDDD-DDDD-DDDDDDDDD)
```

So it's not possible to fix it so far, as my tool built on-top of Facebook's Node.JS tool chain.
According to
https://reactnative.dev/docs/running-on-device#running-your-app-on-ios-devices
you have to use Xcode to run in your device.
By a temp solution, you can run it through Xcode one time, after that disconnect it,
using my tool windows to start the React Packager tool, then double shake in device to connect to the metro server.