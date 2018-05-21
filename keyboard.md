---
layout: default
ref: keyboard
lang: en
---

## Church Slavonic Keyboard Drivers

Keyboard drivers are the next thing you need after a font in order to work with Church Slavonic text. 
Entering text using the Character Map (or some similar utility) is not just slow, it can also cause problems like 
improper positioning of diacritical marks. Several different options are available for entering Church Slavonic text on 
the keyboard. 

### Virtual keyboards

A virtual keyboard allows you to type Church Slavonic text without installing any software.
Just enter the text into your browser and then copy/paste it into a text editor or generate
a PDF for printing.

* [Church Slavonic virtual keyboard](https://www.ponomar.net/cu_vkeyb.html)

### Installable keyboard drivers

Keyboard drivers can be installed on your computer.
The **Russian Extended** keyboard allows you to enter Russian text on the standard Russian
ЙЦУКЕН keyboard and provides Church Slavonic characters on Level 3 (AltGr).
The **Russian Phonetic** keyboard offers the same functionality, but using the phonetic
Russian (ЯВЕРТЫ) layout. The **Church Slavonic** keyboard is a completely new layout
optimized for entering Church Slavonic text. A Church Slavonic **Glagolitic** keyboard
is also available for entering Glagolitic text (only for GNU / Linux systems).

Read [the documentation](https://www.ponomar.net/files/docen.pdf)
for more information and installation instructions.

#### Windows

* [Russian Standard (ЙЦУКЕН) Extended](https://www.ponomar.net/files/ru-ext.zip)
* [Russian Phonetic (ЯВЕРТЫ) Extended](https://www.ponomar.net/files/ru-phonx.zip)
* [Special Church Slavonic](https://www.ponomar.net/files/cu-kbd.zip)

#### Apple OS X

* [Russian Extended](https://www.ponomar.net/files/ru-ext_mac.zip)
* [Special Church Slavonic](https://www.ponomar.net/files/cukeyb_mac1.zip)

#### GNU / Linux

All layouts are available via the m17n-cu package.

* For **Debian-based systems** such as Ubuntu and Linux Mint, add the SCI repository
to your /etc/apt/sources.list file:

  ```
  deb http://www.ponomar.net/apt/ ./ # Slavonic Computing Initiative
  ```

* Import the verification key:

  ```
  wget -q http://www.ponomar.net/apt/public.gpg -O- | sudo apt-key add -
  ```

* Update your software sources:

  ```
  sudo apt-get update
  ```

* Install our package:

  ```
  sudo apt-get install m17n-cu
  ```

* For **all other systems**, [download](https://github.com/typiconman/m17n-cu/releases)
the m17n-cu tarball and install its contents.

You will then need to set up IBUS to be your input method and select the wanted
keyboard layout from the m17n database.
See the [the documentation](https://www.ponomar.net/files/docen.pdf)
for more information.

#### Android

Physical Keyboard Driver for USB/Bluetooth keyboards:
[download APK](https://www.ponomar.net/files/cu-android.apk)
**Warning**: this is alpha phase software and is intended for testing purposes only!

#### Documentation

Documentation for all keyboard layouts and installation instructions in PDF: [download](https://www.ponomar.net/files/docen.pdf)

#### FAQ's

* The license for keyboard drivers [is indicated on the legal page](legal.html)

* If you have questions, [ask the SCI-users mailing list](support.html).

