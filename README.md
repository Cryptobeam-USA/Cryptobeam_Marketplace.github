# Cryptobeam Marketplace App

Welcome to the Cryptobeam Marketplace app.

## What is Cryptobeam Marketplace?

Welcome to Cryptobeam CEX - the cutting-edge centralized exchange platform designed for the modern trader. Our platform offers a robust, secure, and intuitive interface for trading a wide array of cryptocurrencies. Experience swift transactions, real-time analytics, and comprehensive customer support. Join the Cryptobeam CEX community and take your trading to the next level.

### Useful Links

@@ -34,9 +38,7 @@ Welcome to Cryptobeam CEX - the cutting-edge centralized exchange platform

[App Dashboard](https://app.cryptobeam.us/)
·
[Knowledgebase](https://knowledge.cryptobeam.us/)
·
[Developer Training](https://knowledge.cryptobeam.us.com/cryptobeam-developer-training)
·
[Forum](https://discuss.cryptobeam.us/)
·
[Tech Support](https://cryptobeam.us.slack.com/archives/CGSAV319V)

## Table of Contents

1. [Project Description](#project-description)
2. [Project Structure](#project-structure)
3. [Modules](#modules)
4. [Getting Started: Frontend](#getting-started-frontend)
   - [Installation](#installation)
   - [Running with Fastlane](#running-with-fastlane)
     - [Android](#android-1)
     - [iOS](#ios-1)
     - [React Native Web](#react-native-web)
5. [Getting Started: Backend](backend#readme)
6. [License](#license)

## Project Description

Cryptobeam is a premier application engineered utilizing the robust capabilities of Chronicle OpenHFT for high-performance computing and CCXT for a comprehensive cryptocurrency exchange trading library. This fusion of technologies ensures that Cryptobeam provides an exceptional, efficient, and secure trading environment, catering to the diverse needs of the modern cryptocurrency market. Embrace the future of trading with Cryptobeam, where technology meets opportunity.

Cryptobeam leverages the power of .NET microservices, ensuring scalable and reliable performance tailored to trading needs. It integrates FIX/quickFIX language protocols for standardized communication and utilizes the robust infrastructure of AWS Cloud for unparalleled uptime and global reach. Built on a diverse technological stack including Java, Python, and C++, Cryptobeam offers a versatile and powerful trading platform. Experience the pinnacle of trading technology with Cryptobeam, where advanced engineering meets market demands.

## Project Structure

    .
    ├── ...
    ├── android                 # Android native files
    ├── backend                 # Django backend REST API
    ├── ios                     # iOS native files
    ├── modules                 # Modules
    ├── public
    ├── screens
    ├── store                   # Application state storage
    ├── ...
    ├── README.md
    └── ...

## Modules (THIS SECTION IS AUTO-GENERATED, PLEASE DO NOT EDIT)

This section will show any installed modules you add from the Storyboard Modules section.
- [react-native-2fa](modules/2fa)
- [react-native-address-selection-google-autocomplete](modules/address-selection-autocomplete)

# Getting started: Frontend

This section outlines instructions on setting up a local development environment for the frontend of your application.

## Installation

### Metro

After cloning the repo, install the dependencies locally with [Yarn](https://yarnpkg.com/):

```sh
yarn install
```

Start your [Metro](https://facebook.github.io/metro/) server:

```sh
npx react-native start
```

### Android

```sh
npx react-native run-android
```

### iOS

```sh
pod install --repo-update --project-directory=ios
npx react-native run-ios
```

### Setup react-native-vector-icons

Follow instructions at their [README.md](https://github.com/oblador/react-native-vector-icons/blob/master/README.md#installation)

## Running with Fastlane

[Fastlane](https://fastlane.tools/) makes testing, building, and deploying apps
easier.

Install fastlane globally (`npm i -g fastlane` or `yarn i -g fastlane`).
Android and iOS dependencies are the same as React Native CLI.

All fastlane commands are run from the platform directory. For example, Android
commands must be run from `android/`. Fastlane should be executed using `bundle exec` to ensure dependencies are managed correctly.

The commands for Android and iOS are the same:

- Run tests: `bundle exec fastlane tests`
- Local build: `bundle exec fastlane build`
- Build and upload a beta (requires signing): `bundle exec fastlane beta`
- Build or promote a release: `bundle exec fastlane deploy`

### Android

Publish an Android app you must first create an app in the Play Console and
manually upload an APK. After the first upload run `bundle exec fastlane supply init` from `android/` to sync with the Play store. All future releases will be
uploaded automatically.

Android uses tracks. A beta release will build the app and upload to the beta
track. Deploying will promote from beta to production.

### iOS

CB developers must follow fastlane's [codesigning guide](https://codesigning.guide/) for using match.
Match will automatically sign iOS builds.

New CB developers should get access to the codesigning repo and run `bundle exec fastlane match development` from `ios/`.

Not a CB developer? Create an [Apple developer](https://developer.apple.com)
and follow the instructions on [codesigning guide](https://codesigning.guide/)
to setup your certificates.

## React Native Web

You can build and deploy your React Native app in the web too!

To get started run:

```sh
yarn run web
```

This will start a local development server so that you can iterate and preview your changes. Visit it at [localhost:8080](http://localhost:8080).

To build the web version of the project you can run:

```sh
yarn run web:build
```

And then commit/push the output created at `backend/web_build` to the git repository.

# License

The use of code in this repository is governed by Cryptobeam [Terms and Conditions](https://www.cryptobeam.us/terms-of-service).

Created with ❤️ by [Cryptobeam](https://www.cryptobeam.us/)
