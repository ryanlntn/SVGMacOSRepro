# Minimal reproduction of https://github.com/software-mansion/react-native-svg/issues/2192

Steps to create this repo:

1. Install RN compatible with RN MacOS
2. Install RN MacOS
3. Install RN SVG

Steps to reproduce:

1. Clone this repo
2. `yarn install`
3. `cd macos && RCT_NEW_ARCH_ENABLED=1 pod install`
4. `cd .. && yarn macos`

The build fails with `Property 'center' not found on object of type 'RNSVGUse *'`.
