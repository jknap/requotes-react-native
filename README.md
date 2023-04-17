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
1. Create the `assets` folder under `./android/app/src/main/`
```bash
mkdir android/app/src/main/assets
```
2. Generate the bundle file for android:
```bash
npx react-native bundle --platform android --dev false --entry-file index.js --bundle-output android/app/src/main/assets/index.android.bundle --assets-dest android/app/src/main/res
```
3. Launch Android Studio and open the project for your application (more specifically the `android` folder of you React Native project)
4. Build the .apk file:
![](https://github.com/jknap/requotes-react-native/blob/main/readme-assets/build-a-dot-apk-in-android-studio.png)