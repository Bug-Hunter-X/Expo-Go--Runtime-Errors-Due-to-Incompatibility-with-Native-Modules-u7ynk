# Expo Go Incompatibility with Native Modules

This repository demonstrates a common error encountered when using Expo Go to test applications that rely on native modules. Expo Go has limitations on the native modules it can support. Attempting to use an unsupported module results in runtime errors.

## Reproducing the Error

The `bug.js` file contains code that uses a hypothetical native module. When this application is run in Expo Go, it will fail.

## Solution

The `bugSolution.js` file provides a workaround.  The solution involves either finding an Expo-compatible alternative or, if necessary, ejecting from the Expo workflow to manage native modules directly.

## Possible Solutions

* **Use Expo Modules:** Explore whether Expo provides a compatible module that offers similar functionality to the unsupported native module.  Expo's documentation lists its supported modules.
* **Eject from Expo:**  This is a more advanced and potentially disruptive solution. It involves removing Expo's build system and managing the React Native application entirely yourself. This grants you complete control over native modules, but it also increases the complexity of development and maintenance.