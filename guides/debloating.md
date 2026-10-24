# Debloating

This guide will assist you in disabling the bulls#!t Xiaomi puts on your phone.

## Table of Contents
- [First Steps](#first-steps)
- [Setting Up](#setting-up)
- [Using Canta](#using-canta)

> [!TIP]
> Emoji Legend
> 
> ⭐ - Recommended
> 
> 🌐 - Indexes
>
> ⚠️ - Warning (Untested, sketchy, dangerous, or recently involved with controversies. Will vary from case from case)

## First Steps
Before doing anything, it is necessary to turn on Developer Options, USB Debugging and/or Wireless debugging. Those
later 2 features are sadly locked unless you have logged in to your Xiaomi account, and can only be bypassed with root.

### Turning on Developer Options

1. Go to settings -> About Phone, and spam-click on OS Version
2. Insert your passcode / password / pattern
3. go back, head to the bottom of the settings page -> Additional Settings -> Developer Option

There are a lot of options there, so a rule of thumb is to not mess around unless you know what you are doing / understood what said option does. Next, we will allow our phone to accept commands (aka ADB: Google's Android Device Bridge) from other devices and from the network.

### Tuning on USB debugging, Wireless Debugging, USB Debugging (Security settings), and Install via USB

Despite Xiaomi's attempt to scare you off with their giant red alert screen, it is safe to turn on as long as you know what you are doing

1. go to Developer Options -> USB Debugging
2. Toggle it on
3. Wait for 10 seconds, check "I'm aware of the possible risks, and assume...", then click the red OK button
4. Follow the same process for Wireless Debugging, USB Debugging (Security settings), and Install via USB

## Setting Up
For debloating, we can use the Canta app, which can uninstall any app via ADB. For that, first we will have to set up Shizuku, which allows android apps to use the System API. We can also use Universal Android Debloater Next Generation, which is basically the same thing, but on a computer instead.

### Choosing a shizuku flavor
Shizuku itself hasn't been updated in a while, and is broken on Android 17. While functional on other versions, its recommended to use something else. [Timeschneeb's](https://github.com/timschneeb) [Awesome Shizuku](https://github.com/timschneeb/awesome-shizuku#shizuku-implementations) has a pretty good list of Shizuku implementations. For this guide and others, we will be using Thedjchi's fork, but any other fork should work more or less the same.

### Setting up Shizuku
Shizuku has 3 different starting methods:

1. "Start by connecting to a computer", that requires you to plug-in your phone to a PC and run a ADB command.
2. "Start via wireless debugging", which after paired will automatically execute the same commands as the PC, but locally.
3. "Start (for rooted devices), which only appears if the app has SuperUser access, and will start the app without any more setup .

<!--We will disconsider the root method, since if you are reading this, you probably haven't rooted your phone yet.
*TODO: The app itself is pretty straightforward, and guides the user nicely. For now, we will assume the user already set up Shizuku until we get their respective guides ready*-->

<!--### Setting Up Android Device Bridge (ADB) on a computer-->

### Setting up Canta
Install [Canta](https://samolego.github.io/Canta/), authorize it in Shizuku, and you're ready to go.

### Setting up bullshit
Setting it up is as simple as downloading [Universal Android Debloater Next Generation](https://github.com/Universal-Debloater-Alliance/universal-android-debloater-next-generation), and making sure you have ADB on your PC, and USB Debugging on your phone.

## Using Canta
The app is really straightforward: Select the apps you want to uninstall, and click the trashcan icon in the bottom. Each (or at least most) apps are labeled according to their degree of impact on the system. Clicking on a app gives you a description of what the app does, and impacts it can have on your phone if removed, most tested by someone before. A good rule of thumb is to just click on each app, see what it does, its risks, and if you plan to use it. You can filter by tag if you wish. <!--TODO: Add presets so users don't have to do it manually.!-->

## Using Universal Android Debloater Next Generation
Universal Android Debloater works almost exactly like Canta. To use it, start by plugging in your android device in you PC, and opening the program. The app has virtually all the same functions as Canta. Select the apps you want to uninstall, click in "Review selection", do as the button say, and click apply.
