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
    

## [Semantic Versioning](https://semver.org) - Given a version number MAJOR.MINOR.PATCH, increment the:

MAJOR version when you make incompatible API changes,
MINOR version when you add functionality in a backwards compatible manner, and
PATCH version when you make backwards compatible bug fixes.
Additional labels for pre-release and build metadata are available as extensions to the MAJOR.MINOR.PATCH format.