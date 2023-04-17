# Build an iOS Simulator .app in a React Native project

1. Generate the bundle file for ios:
```bash
npx react-native bundle --entry-file='index.js' --bundle-output='./ios/main.jsbundle' --dev=false --platform='ios'
```
2. Launch Xcode and open the workspace for your application.
![alt text](https://github.com/jknap/requotes-react-native/blob/main/readme-assets/open-a-workspace-on-xcode.png)
3. Follow these steps to generate the .app file:
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
3. Go to the `android` folder:
```bash
cd android
```
4. Build the .apk file:
```bash
./gradlew assembleDebug
```
5. Your .apk file will be located in `./android/app/build/outputs/apk/debug/app-debug.apk`. You can use an Android emulator to validate it.
![](https://github.com/jknap/requotes-react-native/blob/main/readme-assets/validate-a-dot-apk-file-with-an-Android-emulator.gif)
