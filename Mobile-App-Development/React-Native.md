# React Native

[Official docs on React Native](https://facebook.github.io/react-native/docs/getting-started)

Using Expo CLI:
* Start a new app by typing:
```
expo init AwesomeProject

cd AwesomeProject
npm start # you can also use: expo start
```
## Network Requests
* There are two ways to make a network request in React Native
  * fetch
    * Built in function for making network requests
    * Error handling is a bit weird
    * Requires us to write a lot of wrapper code to make it work 'sensibly'
  * axios
    * Separate library for making requests
    * Easy to use, sensible defaults
    * Increases app size (very slightly)
    