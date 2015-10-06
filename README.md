# Basic Push Notifications Sample App for PhoneGap/Cordova

<a href="https://platform.telerik.com/#appbuilder/clone/https://github.com/telerik/backend-services-push-hybrid.git" target="_blank"><img src="http://docs.telerik.com/platform/appbuilder/sample-apps/images/try-in-appbuilder.png" alt="Try in AppBuilder" title="Try in Telerik Platform" /></a> <a href="https://github.com/telerik/backend-services-push-hybrid" target="_blank"><img style="padding-left:20px" src="http://docs.telerik.com/platform/appbuilder/sample-apps/images/get-github.png" alt="Get from GitHub" title="Get from GitHub"></a>

* [Overview](#overview)
* [Screenshots](#screenshots)
* [Requirements](#requirements)
* [Configuration](#configuration)
* [Running the Sample](#running-the-sample)
* [See Also](#see-also)

## Overview

This repository contains a basic sample app that can receive push notifications sent from its Telerik Platform backend. It is a hybrid app built using Telerik AppBuilder and Cordova.

The sample app utilizes the following Telerik products and SDKs:

- [Telerik Backend Services](http://docs.telerik.com/platform/backend-services/)&mdash;this is the backend of Telerik Platform where you can store data, files, and user accounts as well as set up and send push notifications
- [Telerik Backend Services JavaScript SDK](http://docs.telerik.com/platform/backend-services/javascript/getting-started-javascript-sdk)&mdash;to connect the app to Telerik Backend Services
- [Telerik Push Plugin](https://github.com/Telerik-Verified-Plugins/PushNotification) for AppBuilder&mdash;to enable push notifications in Cordova

## Screenshots

Initial View|After Device is Registered
---|---
![Before Registering](https://raw.githubusercontent.com/telerik/backend-services-push-hybrid/master/screenshots/android-before-registering.png)|![After Registering](https://raw.githubusercontent.com/telerik/backend-services-push-hybrid/master/screenshots/android-after-registering.png)

## Requirements

Before you begin, you need to ensure that you have the following:

- **An active [Telerik Platform](https://platform.telerik.com) account**
Ensure that you can log in to a Telerik Platform account. This can be a free trial account.
- **Telerik AppBuilder**
The sample app requires Telerik AppBuilder to run. This can be the in-browser client, the desktop client or the extension for Visual Studio.

## Configuration

The sample app comes fully functional, but to see it in action you must link it to your own Telerik Platform account.

1. Click the "Try in AppBuilder" button to clone the repository in AppBuilder.<br>
	An app called "My App" is created for you with an AppBuilder project set up.
2. Click **My App** in the navigation bar at the top to go the app home.
3. Create a Backend Services project. If you want to have sample data preloaded, select the **Start from the Friends app** option. Otherwise select the **Start from scratch** option.
4. Once the Backend Services project is ready, go to **Overview > API Keys**.
5. Take note of your API Key.
6. Go back to the AppBuilder project.
7. Open the `/scripts/app/main.js` file.
8. Locate the `bsApiKey` variable and replace its value with the Backend Services API Key that you acquired earlier.
9. If you want to run the app on Android devices, locate the `googleApiProjectNumber` variable and replace its value with your Google project number. More details on obtaining the project number can be found on [Google Developers](https://developers.google.com/console/help/new/#projectnumber).
10. Finally, set up push notifications in your Backend Services project as explained in [Enabling Push Notifications](http://docs.telerik.com/platform/backend-services/javascript/push-notifications/push-enabling).

## Running the Sample

Once the app is configured, you can run it on a real device. To run it, follow the steps in the product's documentation: [Running Apps on Devices](http://docs.telerik.com/platform/appbuilder/testing-your-app/running-on-devices/working-with-devices).

> When running the app, ensure that you are building it as an app package as opposed to an AppBuilder companion app package.

> Push notifications are not supported when running the app on device simulators/emulators. 

> Ensure that the device that you are using has Internet connectivity when running the sample.

## See Also

[Getting Started with Push Notifications](http://docs.telerik.com/platform/backend-services/javascript/push-notifications/push-getting-started)
