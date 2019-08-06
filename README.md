# react-native-hello-world

## Getting started

`$ npm install react-native-hello-world --save`

### Mostly automatic installation

`$ react-native link react-native-hello-world`

### Manual installation


#### iOS

1. In XCode, in the project navigator, right click `Libraries` ➜ `Add Files to [your project's name]`
2. Go to `node_modules` ➜ `react-native-hello-world` and add `HelloWorld.xcodeproj`
3. In XCode, in the project navigator, select your project. Add `libHelloWorld.a` to your project's `Build Phases` ➜ `Link Binary With Libraries`
4. Run your project (`Cmd+R`)<

#### Android

1. Open up `android/app/src/main/java/[...]/MainApplication.java`
  - Add `import com.reactlibrary.HelloWorldPackage;` to the imports at the top of the file
  - Add `new HelloWorldPackage()` to the list returned by the `getPackages()` method
2. Append the following lines to `android/settings.gradle`:
  	```
  	include ':react-native-hello-world'
  	project(':react-native-hello-world').projectDir = new File(rootProject.projectDir, 	'../node_modules/react-native-hello-world/android')
  	```
3. Insert the following lines inside the dependencies block in `android/app/build.gradle`:
  	```
      compile project(':react-native-hello-world')
  	```


## Usage
```javascript
import HelloWorld from 'react-native-hello-world';

// TODO: What to do with the module?
HelloWorld;
```
