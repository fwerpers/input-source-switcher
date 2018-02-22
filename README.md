Command line input source switcher for Mac.
===========================================

About
-----
Fork from https://github.com/vovkasm/input-source-switcher. Wanted a command for toggling between keyboard layouts and made changes accordingly.

This small utility for Apple OS X allows to easily switch input sources from a command line.

~~It's main purpose is to be used as a service in [vim-xkbswitch](https://github.com/lyokha/vim-xkbswitch) plugin.~~

Usage
-----

    issw [-h] [-l] [<input-source-id>]

    -h - show help message
    -l - list all selectable input sources
    -V - print version number

If no arguments are specified, it ~~prints the current input source~~ selects the next keyboard layout as input source.
If `<input-source-id>` is specified, it selects the specified input source.

How to build
------------

    git clone https://github.com/vovkasm/input-source-switcher.git
    cd input-source-switcher
    mkdir build && cd build
    cmake ..
    make
    make install

How to develop with Xcode
-------------------------

    cd input-source-switcher
    mkdir xcode && cd xcode
    cmake -G Xcode ..
    open InputSourceSwitcher.xcodeproj

Main author
------

Vladimir Timofeev

Licensing
---------

This projected is licensed under the terms of the MIT license.

