# react-native-init-web3
Boilerplate proyect using react native and web3 from scratch

# How do i set up?

1. yarn install
2. react-native run-android or react-native run-ios 

# How to support web3js 1.0?

1. Added node-libs-browser to support the crypto module
2. Added rn-cli.config.js, a file that allows to add extra modules
3. Since web3js is browser-based, it has some variables like "btoa", that are part of browsers standards (https://developer.mozilla.org/pl/docs/Web/API/WindowBase64/btoa), so, there is a global.js file that create that function and put it in a global scope for the application.

# Known Issues

1. Currently working with web3js 1.0-beta34, but, for beta35 and 36 there is an error that doesnt allow to connect to a provider. 
Same error as this: https://ethereum.stackexchange.com/questions/59240/can-not-connect-to-infura-service-in-web3-js
