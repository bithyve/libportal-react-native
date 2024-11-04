# libportal-react-native


`libportal-react-native` is a React Native library developed to integrate [TwentyTwo Portal](https://github.com/TwentyTwoHW/portal-software/tree/master) functionality into mobile applications for React Native environments.


## Installation

To add `libportal-react-native` to your project, follow these steps:

### Step 1: Install via `package.json`

Add `libportal-react-native` as a dependency in your `package.json`:

```json
"dependencies": {
  "libportal-react-native": "git+https://github.com/bithyve/libportal-react-native.git"
}
```

### Step 2: Then run
  ```
  npm install
  ```
  or

  ```
  yarn install
  ```

### Step 3: Ensure your project meets the following iOS requirements:

- Deployment target of at least iOS 13.0.
- CocoaPods installed for iOS dependencies.

Run the following command to install the iOS dependencies:  
```
cd ios
pod install
```
  


## Usage

```js
import {
  PortalSdk,
  type CardStatus,
} from 'libportal-react-native';



const sdk = new PortalSdk(true);
// ...
export const getStatus = async (): Promise<CardStatus> => {
  return sdk.getStatus();
};

```
---
