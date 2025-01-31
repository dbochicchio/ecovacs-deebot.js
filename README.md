![Logo](ecovacs-deebot.png)

# ecovacs-deebot.js

[![npm](http://img.shields.io/npm/v/ecovacs-deebot.svg)](https://www.npmjs.com/package/ecovacs-deebot)
[![npm](https://img.shields.io/npm/dm/ecovacs-deebot.svg)](https://www.npmjs.com/package/ecovacs-deebot)
[![npm](https://img.shields.io/npm/dt/ecovacs-deebot.svg)](https://www.npmjs.com/package/ecovacs-deebot)
[![Dependency Status](https://img.shields.io/david/mrbungle64/ecovacs-deebot.js.svg)](https://david-dm.org/mrbungle64/ecovacs-deebot.js)
[![Travis-CI](https://travis-ci.org/mrbungle64/ecovacs-deebot.js.svg?branch=master)](https://travis-ci.org/mrbungle64/ecovacs-deebot.js)

Library for running Ecovacs Deebot vacuum cleaner robots

## Installation

Information on how to install this library can be found [here](https://github.com/mrbungle64/ecovacs-deebot.js/wiki/Installation).

It is recommended to use version 10.x, 12.x or 14.x of Node.js. The minimum required version is 10.x

## Usage

Information on how to use this library can be found [here](https://github.com/mrbungle64/ecovacs-deebot.js/wiki/Usage).

## Models

### Supported models

* Deebot 900/901
* Deebot OZMO 930
* Deebot OZMO 920/950

The models listed are those that I have in use myself or which are technically identical to these.

### These models should work properly or at least partially

* Deebot Slim 2
* Deebot N79 series
* Deebot M88
* Deebot 600/601/605
* Deebot 710/711/711s
* Deebot OZMO 610
* Deebot OZMO 900/905
* Deebot OZMO Slim 10
* Deebot OZMO T5
* Deebot OZMO T8 series
* Deebot OZMO T9 series
* Deebot N3 MAX
* Deebot N7
* Deebot N8 series
* Deebot U2 series

The models listed are either already known to work or are technically similar to these models.
Nevertheless, the functionality may be partially limited.

I try to achieve a wide range of functionality, but decide this case by case depending on complexity and various other criteria.
There is of course no claim to full functionality.

## Known issues

* There's a strange behavior of the battery value on Deebot 900/901. It's very likely that this is a firmware bug
* Some cleaning commands may not work with Deebot 710/711/711s
* "Edge" command does not work with Deebot U2 (starts auto clean instead)

## Changelog

### 0.6.1 (alpha)
* Added full map data (maps, spot areas, virtual boundaries) as one structured event
* (boriswerner) Initial implementation of a static image of the map
* Handle compressed spot area boundary data (e.g. T9 series)
* Handle custom names for spot areas (e.g. T9 Series)
* Some enhancements and fixes

### 0.6.0
* Updated login process (credits to [@And3rsL](https://github.com/And3rsL))
* Support for Chinese server login
* Implemented AutoEmpty commands for T8+/plus
* Added some cleaning log values and cleaning stats
* Initial support for some more models (e.g. N3, N7, N8, T9 series)
* Improved example apps
* (dbochicchio) Added some structured events
* Quite a lot refactoring and code consolidation
* Several improvements and fixes
* Bump some dependencies

### 0.5.6
* Some improvements for handling charge status

### 0.5.5
* Added OZMO T5 and some more T8 models
* Several enhancements and fixes

### 0.5.4
* Some fixes for cleaning logs (non 950 type)

### 0.5.3
* Some refactoring and code improvements

### 0.5.2
* Implement ResetLifeSpan, SetVolume and GetVolume for 950 type models
* Implement OnOff for non 950 type MQTT models
* Implement method to get translated spot area names
* Bump some dependencies
* Several enhancements and fixes

### 0.5.1
* Initial support for Deebot U2 series
* Improved support for T8 models
* Improved handling of device classes
* (boriswerner) Fixed cleaning log for 950 type models
* (boriswerner) VirtualBoundaries handling

### 0.5.0
* Lots of code refactoring
* Fix problem running multiple devices
* Added support for more Ozmo T8 models

### 0.0.2 - 0.4.26
* [Changelog archive](https://github.com/mrbungle64/ecovacs-deebot.js/wiki/Changelog-(archive))

## Thanks and credits

* @joostth ([sucks.js](https://github.com/joostth/sucks.js))
* @wpietri ([sucks](https://github.com/wpietri/sucks))
* @bmartin5692 ([sucks](https://github.com/bmartin5692/sucks), [bumber](https://github.com/bmartin5692/bumper))
* @Ligio ([ozmo](https://github.com/Ligio/ozmo))
* @And3rsL ([Deebotozmo](https://github.com/And3rsL/Deebotozmo))

All credits for originally figuring out and documenting the protocol go to [@wpietri](https://github.com/wpietri).
He documented his [findings on the protocol](http://github.com/wpietri/sucks/blob/master/protocol.md) in his repository.

## Disclaimer

I am in no way affiliated with ECOVACS.

## License

GNU GENERAL PUBLIC LICENSE

Copyright (c) 2021 Sascha Hölzel <mrb1232@posteo.de>
