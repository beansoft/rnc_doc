[//]: # (title: Install React Native Console)

# Install React Native Console

## Prerequisites

1. A JetBrains IDE 2020.3+

Install an IDE if you don't have one from [Jetbrains](https://www.jetbrains.com/?from=ReactNativeConsole)
or [Android Studio](https://developer.android.com/sdk/installing/studio.html). RN Console supports all major Jetbrains

IDEs include IDEA CE, IDEA Ultimate, WebStorm, Android Studio, PhpStorm, RubyMine and GoLand and so on.


> The difference in these IDEs is that only paid IDE supports advanced JavaScript editor and in-IDE debugger, please see: [Developing mobile apps with React Native in WebStorm](https://blog.jetbrains.com/webstorm/2016/12/developing-mobile-apps-with-react-native-in-webstorm/).
> For more info about WebStorm and React Native, please visit: <a href="https://www.jetbrains.com/help/webstorm/react-native.html">https://www.jetbrains.com/help/webstorm/react-native.html</a>.
>
{style="note"}

2. Node.js

   If you are only going to dev apps with [Expo](https://expo.dev/), then you only need to
   have [Node 14 LTS](https://nodejs.org/en/download/) or greater installed, you can use npm to install the Expo CLI
   command line utility: `npm install -g expo-cli` .

3. Android or iOS development env setup

   Please check for [Setting up the development environment](https://reactnative.dev/docs/environment-setup) for more
   info.

   > **Note for Mac M1 users**
   >
   > Mac M1 architecture is not directly compatible with Cocoapods. If you encounter issues when installing pods, you
   can solve it by running:
   >
   >
   > ```shell
    > sudo arch -x86_64 gem install ffi
    > arch -x86_64 pod install
    > ```
   >
   > These commands install the `ffi` package, to load dynamically-linked libraries and let you run the `pod install`
   properly, and runs `pod install` with the proper architecture.


4. Optional: Download and install [Genymotion Desktop](https://www.genymotion.com/download/)

   Genymotion Virtual Devices is an Android emulator. RN Console integrates the support for Genymotion Desktop with all
   versions of Android Studio, IDEA or WebStorm since 2020.3.

   > Genymotion needs an account to work, using it please follow the official
   guide: https://docs.genymotion.com/desktop/.

5. Optional: Download and install [React Native Debugger](https://github.com/jhen0409/react-native-debugger/releases)

   React Native Debugger is a free and opensource standalone app based on official debugger of React Native, and
   includes React Inspector / Redux DevTools, allow you to debug your React Native app without using WebStorm or IDEA
   Ultimate. More info, please visit: https://github.com/jhen0409/react-native-debugger/tree/master/docs .

[//]: # "   ### Core Features"

[//]: # "   "

[//]: # "   **Powerful Native Toolkit —** It has a built-in set of tools such as UI analyzer, breakpoint and network inspectors. These tools can come in handy for any user. It doesn’t matter whether you are an amateur or an expert."

[//]: # "   "

[//]: # "   **Network Inspector —** The Inspector can monitor both inbound and outbound traffic to understand the load."

[//]: # "   "

[//]: # "   **Constant Statistics —** Tracking such variables means that statistics are available for the owner to understand where the content is lacking. And where it currently stands in terms of infrastructure and audience."

[//]: # "   "

[//]: # "   **UI Assistance —** The built-in assistance can help in understanding the usability, readability of the application and overall interface."

6. Hermes engine

   The Hermes engine is an open source JavaScript engine created by Facebook to optimize building and running React
   Native applications. It improves app performance and decreases app size.

   Click [here](https://reactnative.dev/docs/hermes) to learn more about Hermes and how to enable it for your
   application.

## Check the required tools

RN Console relies on top of various tools to work properly.

- Expo

  Only Node.js is required, bring up a terminal and enter following command to check: `npm`

  The output should be something like this:

  ```
  npm <command>
  
  Usage:
  
  npm install        install all the dependencies in your project
  npm install <foo>  add the <foo> dependency to your project
  npm test           run this project's tests
  npm run <foo>      run the script named <foo>
  npm <command> -h   quick help on <command>
  npm -l             display usage info for all commands
  npm help <term>    search for help on <term> (in a browser)
  npm help npm       more involved overview (in a browser)
  ```

- Android Development

  Have the [`emulator`](https://developer.android.com/studio/run/emulator-commandline) utility available in your `PATH`
  if you're developing Android applications;

  Have the [`adb`](https://developer.android.com/studio/command-line/adb) utility available in your `PATH` if you're
  developing Android applications;

  To start an emulator in WebStorm / IDEA throught RN Console, launch Android Studio and choose
  menu `Tools > AVD Manager` to create at lease
  one Android virtual device. This is a one-time task to do, after that you can close the Android Studio.

  > On Mac or Linux platform:
  >
  > If you can't find adb, try this shell command:
  > `sudo ln -s ~/Android/Sdk/platform-tools/adb /usr/bin/adb`
  > If you can't find avd list, try this shell command(please ensure your emulator path):
  > `sudo ln -s ~/Library/Android/sdk/emulator/emulator /usr/bin/emulator`
  > More info please ref this issue:
  > https://github.com/beansoft/react-native-console/issues/17

- iOS Development

  Have the `xcodebuild` utility available in your `PATH` if you're developing iOS applications;

  Have the [`adb`](https://developer.android.com/studio/command-line/adb) utility available in your `PATH` if you're
  developing Android applications;

## Install plugin from IDE

1. Open your IDE and press Ctrl+Alt+S to open the IDE settings.

2. Select **Plugins**, click the Marketplace tab and enter: `React Native Console`

3. Click **Install** to install the plugin and restart your IDE if prompted.

![](rnconsole-install-dark.png){thumbnail="true" thumbnail-same-file="true" width="1942" height="606"}



## Download and install plugin from disk

1. Download the latest plugin version from https://plugins.jetbrains.com/plugin/9564-react-native-console/versions

2. Open your IDE and press Ctrl+Alt+S to open the IDE settings.

3. Select **Plugins**, click  ![](gearPlain_dark.svg) and then click **Install Plugin from Disk**.

4. Select the plugin archive file and click **OK**.

5. Click **OK** to apply the changes and restart your IDE if prompted.

