# Build an iOS Simulator .app in a React Native project

1. Generate the bundle file for ios:
```bash
npx react-native bundle --entry-file='index.js' --bundle-output='./ios/main.jsbundle' --dev=false --platform='ios'
```
2. Launch Xcode and open the workspace for your application.
![alt text](https://github.com/jknap/requotes-react-native/blob/main/readme-assets/open-a-workspace-on-xcode.png)
3. Follow these steps to generate teh .app file:
![](https://github.com/jknap/requotes-react-native/blob/main/readme-assets/generate-a-dot-app-from-a-react-native-project.gif)
4. Validate your .app file using a simulator:
![](https://github.com/jknap/requotes-react-native/blob/main/readme-assets/validate-a-dot-app-file-with-an-iOS-simulator.gif)

# Build an Android emulator .apk in a React Native project
