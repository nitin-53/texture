---
layout: post
type: tech
author: "fooman"
title:  "How to type in Indic languages on Ubuntu"
description: Typing Indic languages with the help of IBus on Ubuntu or on Linux Mint or on other similar Linux distros.
date:   2020-02-23 18:00:00 +0530
categories: IndianLanguages Ubuntu LinuxMint IBus m17n
---
[IBus](https://en.wikipedia.org/wiki/Intelligent_Input_Bus "wikipedia:IBus") Intelligent Input Bus is an [Input Method](https://wiki.archlinux.org/index.php/Input_method "wikipedia:Input_method") Framework which used to enter non-Latin characters. We will be using IBus to write in Indian Languages. 'm17n' is an Input Method Engine (IME) which allows input of many languages using input methods from 'm17n-db'.

## Step 1: Installing ibus-m17n
open the terminal and run below commands.
```
sudo apt-get install ttf-indic-fonts
sudo apt-get install ibus-m17n
```

### Optional Steps
sometimes more packages needs to be installed on some distros.
```
sudo apt-get install ibus m17n-db m17n-contrib ibus-gtk
sudo apt-get install libm17n-0-dbg libm17n-0 libm17n-im-config0
```

## Step 2: Adding IBus to startup application
From system's 'Setting/Preference', select the 'Startup Applications'. Add a new application; name it 'IBUS' or 'IBus' or 'IBusDaemon' or whatever you like. In command property, type `ibus-daemon`. Now save this setting and Done. Restart the system. Now in system's Setting/Preference' you can find 'Input Method' setting where you can change input methods.

## Step 3: Selecting various input method from IBus preferences.
In system's Setting/Preference' you can find a new setting 'ibus preferences'. In this setting there is a menu on top called 'Input method'. Here you can add different input methods as you like. Default keyboard layout for languages is 'Inscript'. You can find different supported keyboard layouts [here](https://fedoraproject.org/wiki/I18N/Indic#Keyboard_Layouts "keyboard_layouts") by clicking on language name.

## Step 4: Refering to Unicode
You may not find some characters in given layouts for a specific language. These characters can be typed with the help of [Unicode](https://home.unicode.org/basic-info/overview/ "unicode") character codes. You can find Unicode chart [here](http://www.unicode.org/charts/ "unicode_chart") and characters codes can be found by clicking a script name of a desired language. For typing a Unicode character, press <kbd>Ctrl</kbd> + <kbd>Shift</kbd> + <kbd>U</kbd> and type the character code and press <kbd>Space</kbd>. Now, you will see character is printed.

> *If you find any difficulties, then contact me on my email given on blog's home page.*