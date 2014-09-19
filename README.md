# Freebox plugin for QtCreator

## Features

This plugin helps QML application development for Freebox:

* It declares some wizards for new projects;

* It handles `.fbxproject` files;

* It discovers Freebox with developer mode active, and allows remote
  debugging on them.

## Building

Of course, Qt-5.3+ is required (binary distribution for developer is
enough).

You'll need a QtCreator source tree, version **v3.2.0**, and
corresponding build tree.  Clone from [QtCreator's
Git](https://qt.gitorious.org/qt-creator/).

After build of QtCreator v3.2.0, prepare your environment to actually
point to source and build directories:
```
$ export QTC_SOURCE=$PWD/qt-creator-v3.2.0
$ export QTC_BUILD=$PWD/qt-creator-v3.2.0-build
```

Checkout and build this plugin:
```
$ git clone https://github.com/fbx/freebox-qtcreator-plugin.git
$ mkdir freebox-qtcreator-plugin-build
$ cd freebox-qtcreator-plugin-build
$ qmake ../freebox-qtcreator-plugin
$ make -j10
```

Now plugin is installed in your home directory.

## Support

* [Issue tracker on Github](https://github.com/fbx/freebox-qtcreator-plugin/issues)
* `sdk @ freebox.fr`