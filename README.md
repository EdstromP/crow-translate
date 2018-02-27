# Crow Translate

<img src="./data/icons/app/classic.png" height="128" width="128"/>

**Crow Translate** is a simple and lightweight translator programmed in **C++ / Qt** that allows to translate and speak the selected text using the Google Translate API.
You may also be interested in my library [QOnlineTranslator](https://github.com/Shatur95/QOnlineTranslator "A library that provides free use of the Google Translate API for Qt5") used in this project. 

## Contents

* [Features](#features)
* [Default keyboard shortcuts](#default-keyboard-shortcuts)
* [Dependencies](#dependencies)
* [Installation](#installation)

## Features

* Text translation \ speaking in any application that supports text selection
* Translator window with native interface similar to Google Translate
* Highly customizable shortcuts
* Low memory consumption (~19MB)

## Default keyboard shortcuts

You can change these shortcuts in the settings. Some key sequences may not be available due to OS limitations.

### Global

|  Keys                         | Description             |
|-------------------------------|-------------------------|
| <kbd>Alt</kbd> + <kbd>X</kbd> | Translate selected text |
| <kbd>Alt</kbd> + <kbd>C</kbd> | Show main window        |
| <kbd>Alt</kbd> + <kbd>S</kbd> | Speak selected text     |

### In main window

|  Keys                                             | Description               |
|---------------------------------------------------|---------------------------|
| <kbd>Ctrl</kbd> + <kbd>Return</kbd>               | Translate                 |
| <kbd>Ctrl</kbd> + <kbd>S</kbd>                    | Speak input text          |
| <kbd>Ctrl</kbd> + <kbd>Shift</kbd> + <kbd>S</kbd> | Speak translated text     |

## Dependencies

**Arch Linux:** qt5-base qt5-multimedia gst-plugins-good openssl qt5-tools (make)

**Debian:** qt5-default qt5-qmake libqt5x11extras5-dev qtbase5-dev qtbase5-dev-tools qttools5-dev-tools qtmultimedia5-dev gstreamer1.0-fluendo-mp3 qtgstreamer-plugins-qt5 gstreamer1.0-plugins-good gstreamer1.0-alsa

## Installation

### Automatic script

You can use the automatic script that builds **Crow Translate** and creates a package for your distribution:

```bash
cd dist/unix
./create-package
```

Than you can install it as usual. The script will tell you where the package will be after the making. Currently, only **Arch Linux**, **Debian** and their derivatives are supported.

### Arch Linux and derivatives

You can install [crow-translate-git](https://aur.archlinux.org/packages/crow-translate-git "A simple and lightweight translator that allows to translate and speak the selected text using the Google Translate API") from AUR.

### Manual building

You can build **Crow Translate** by using the following commands:

```bash
qmake
make
make clean
```

Then you can use standalone binary `crow`.
