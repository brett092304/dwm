This is my config of dwm window manager. It currently does not have any patches installed but does include my config.h file

dwm - dynamic window manager
============================
dwm is an extremely fast, small, and dynamic window manager for X.


Requirements
------------
In order to build dwm you need the Xlib header files.


Installation
------------
Edit config.mk to match your local setup (dwm is installed into
the /usr/local namespace by default).

Afterwards enter the following command to build and install dwm (if
necessary as root):

    make clean install
    
Then enter the following commands to copy dwm-autostart and dwm-fillbar to /usr/local/bin:

    cp dwm-autostart /usr/local/bin/
    cp dwm-fillbar /usr/local/bin/

Note: You may need to make dwm-autostart and dwm-fillbar executable

If you are running a Display Manger simply copy dwm.desktop to /usr/share/xsessions/:

    cp dwm.desktop /usr/share/xsessions/

If you are **NOT** using a Display Manager then you already know what you are doing


Running dwm
-----------
If you are using a Display Manager then the session "DWM" will be avaible to start at the login screen

To start dwm from the console run:

    startx /usr/local/bin/dwm-autostart -- :[tty you are currently on]


Configuration
-------------
The configuration of dwm is done by creating a custom config.h
and (re)compiling the source code.
