# HMS Analytics Kit iOS Codelab


## Table of Contents

 * [Introduction](#introduction)
 * [Installation](#installation)
 * [Configuration ](#configuration )
 * [Supported Environments](#supported-environments)
 * [Sample Code](#sample-code)
 * [License](#license)
 
 
## Introduction

HUAWEI Analytics Kit offers a rich array of preset analytics models that help you gain a deeper insight into your users, products, and content. With this insight, you can then take a data-driven approach to make informed decisions for product and marketing optimizations.


## Installation

To integrate Analytics Kit, you must complete the following preparations:
*   Create an app in AppGallery Connect, and enable Analytics.
*   Create an Xcode project, and add necessary framework(s).
*   Download configuration file and import into your project.

Edit the Podfile.

Add the pod on which the AppGallery Connect service depends.

    pod 'HiAnalytics'

And run `pod install` command.


## Supported Environments

Xcode 10.1 or a later

iOS 11.0 or later


## Configuration

To activate Analytics Kit, you have to add **agconnect-services.plist** configuration file into your project.

Open your project in AppGallery Connect and Go to **Project Setting** > **General Information**.

In the App information area, download the agconnect-services.plist file.

Import HiAnalytics into your AppDelegate class.

    import HiAnalytics


Call HiAnalytics.config() method in application function.

    HiAnalytics.config()


## Sample Code

Import HiAnalytics into your *ViewController*.

    import HiAnalytics

Call HiAnalytics.onEvent() method in your *ViewController* to post your event.

    HiAnalytics.onEvent("TestEvent", setParams: ["param 1": "value 1"])

Call HiAnalytics.setUserProfile() method in your *ViewController* to post your event.

    HiAnalytics.setUserProfile("favor_sport", setValue: "football")


##  License

HMS Analytics Kit iOS Codelab is licensed under the [Apache License, version 2.0](http://www.apache.org/licenses/LICENSE-2.0).

