# React Native

[Official docs on React Native](https://reactnative.dev/docs)

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

## [App Store Versioning](https://developer.apple.com/library/archive/documentation/General/Reference/InfoPlistKeyReference/Articles/CoreFoundationKeys.html#//apple_ref/doc/uid/20001431-102364)

CFBundleVersion

CFBundleVersion (String - iOS, macOS) specifies the build version number of the bundle, which identifies an iteration (released or unreleased) of the bundle.

The build version number should be a string comprised of three non-negative, period-separated integers with the first integer being greater than zero—for example, 3.1.2. The string should only contain numeric (0-9) and period (.) characters. Leading zeros are truncated from each integer and will be ignored (that is, 1.02.3 is equivalent to 1.2.3). The meaning of each element is as follows:

* The first number represents the most recent major release and is limited to a maximum length of four digits.
* The second number represents the most recent significant revision and is limited to a maximum length of two digits.
* The third number represents the most recent minor bug fix and is limited to a maximum length of two digits.
If the value of the third number is 0, you can omit it and the second period.

While developing a new version of your app, you can include a suffix after the number that is being updated; for example 3.1.3a1. The character in the suffix represents the stage of development for the new version. For example, you can represent development, alpha, beta, and final candidate, by d, a, b, and fc. The final number in the suffix is the build version, which cannot be 0 and cannot exceed 255. When you release the new version of your app, remove the suffix.
