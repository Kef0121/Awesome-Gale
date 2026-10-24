# Debloating

This guide will assist you in disabling the bulls#!t Xiaomi puts on your phone.

## Table of Contents

- [First Steps](#first-steps)

- [Setting Up](#setting-up)

- [Using Canta](#using-canta)

- [Using Universal Android Debloater Next Generation](#using-universal-android-debloater-next-generation)

> [!TIP]
>
> Emoji Legend
>
> ⭐ - Recommended
>
> 🌐 - Indexes
>
> ⚠️ - Warning (Untested, sketchy, dangerous, or recently involved with controversies. Will vary from case to case)

## First Steps

Before doing anything, it is necessary to turn on Developer Options, USB Debugging and/or Wireless debugging. Those later 2 features are sadly locked unless you have logged in to your Xiaomi account, and can only be bypassed with root. So, just go ahead and log into your account. Create one if needed.

### Turning on Developer Options

1. Go to settings -> About Phone, and spam-click on OS Version
2. Insert your passcode / password / pattern
3. go back, head to the bottom of the settings page -> Additional Settings -> Developer Option

There are a lot of options there, so a rule of thumb is to not mess around unless you know what you are doing / understand what said option does. Next, we will allow our phone to accept commands (aka ADB: Google's Android Debug Bridge) from other devices and from the network.

### Turning on USB debugging, Wireless Debugging, USB Debugging (Security settings), and Install via USB

Despite Xiaomi's attempt to scare you off with their giant red alert screen, it is much simpler. All of those options allow for foreign devices to execute commands on our phone. It can be harmful, sure, but if you know what you are doing, you should be good to got

1. go to Developer Options -> USB Debugging
2. Toggle it on
3. Wait for 10 seconds, check "I'm aware of the possible risks, and assume...", then click the red OK button
4. Turn on Wireless Debugging, USB Debugging (Security settings), and/or Install via USB if your chosen method requires them.

## Setting Up

For debloating, we can use the Canta app, which can uninstall preinstalled apps using Shizuku. For that, first we will have to set up Shizuku, which allows Android apps to use some system APIs. We can also use Universal Android Debloater Next Generation, which has a similar purpose but runs on a computer instead.

### Choosing a shizuku flavor

Shizuku compatibility on Android 16 and up has reported issues, and it hasn't been updated in a while. That doesn't necessarily mean the whole app is broken, but forks can be more reliable in the current state. [Timeschneeb](https://github.com/timschneeb)'s [Awesome Shizuku](https://github.com/timschneeb/awesome-shizuku#shizuku-implementations) has a pretty good list of Shizuku implementations. For this guide and others, we will be using [Thedjchi's fork](https://github.com/thedjchi/Shizuku), but other forks may work more or less the same. Check their compatibility and setup instructions, since they can differ.

### Setting up Shizuku

Shizuku has 3 different starting methods:

1. "Start by connecting to a computer", that requires you to plug-in your phone to a PC and run an ADB command.
2. "Start via wireless debugging", which after paired will automatically execute the same commands as the PC, but locally.
3. "Start (for rooted devices)", which only appears if the app has SuperUser access, and will start the app without any more setup.

<!--We will disconsider the root method, since if you are reading this, you probably haven't rooted your phone yet.

*TODO: The app itself is pretty straightforward, and guides the user nicely. For now, we will assume the user already set up Shizuku until we get their respective guides ready*-->

<!--TODO: ### Setting Up Android Debug Bridge (ADB) on a computer-->

### Setting up Canta

Install [Canta](https://samolego.github.io/Canta/), start Shizuku, authorize Canta in Shizuku, and you're ready to go.

### Setting up UADNG

Setting it up is as simple as downloading [Universal Android Debloater Next Generation](https://github.com/Universal-Debloater-Alliance/universal-android-debloater-next-generation), and making sure you have ADB on your PC, and USB Debugging on your phone.

## Using Canta

The app is really straightforward: Select the apps you want to uninstall, and click the trashcan icon in the bottom. Each (or at least most) apps are labeled according to their degree of impact on the system. Clicking on an app gives you a description of what the app does, and impacts it can have on your phone if removed, most tested by someone before. A good rule of thumb is to just click on each app, see what it does, its risks, and if you plan to use it. You can filter by tag if you wish. Recommendations are a guide, not a guarantee that an app is safe to remove on your exact build. <!--TODO: Add presets so users don't have to do it manually.-->

## Using Universal Android Debloater Next Generation
Universal Android Debloater has a similar purpose to Canta, but its interface and recommendations can be quite different. To use it, start by plugging in your android device in your PC, and opening the program. Select the apps you want to uninstall, click in "Review selection", do as the button say, and click apply. Check each package before applying changes; don't assume a preset is safe for every device or software version.
