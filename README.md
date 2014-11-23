linconnect-server
=================

Mirror Android notifications on a Linux desktop.

LinConnect Client: https://github.com/hauckwill/linconnect-client/

LinConnect Server Windows: https://github.com/vikas0380/linconnect-windows

Introduction
------------
LinConnect is a project to mirror *all* Android notifications on a Linux desktop using LibNotify.

*Please note that this is my first time using Python (though I do have experience in other languages), so the code may still be messy. It's a WIP.*

Installation
------------

**Requirements**

* python2
* python-pip
* python-gobject
* libavahi-compat-libdnssd1
* cherrypy (python package)
* pybonjour (python package)

**Running**

Simply run linconnect_server.py to start the server, then start the Android application. The Android application will detect the server and display it in the server list. Selecting it will send a test notification to the server.

**Simple Setup (tested on Ubuntu 13.10)**

Enter the following command into a console to install the server, set it to autostart, and run LinConnect. The server will be automatically updated daily.

```bash
$ wget --quiet https://raw.github.com/hauckwill/linconnect-server/master/LinConnectServer/install.sh; \
chmod +x install.sh; \
./install.sh
```

To remove LinConnect, delete the ~/.linconnect directory.
        
Client Download
---------------

![alt text](https://developer.android.com/images/brand/en_app_rgb_wo_60.png "Google Play")

A binary of the client may be downloaded from the Google Play Store.

https://play.google.com/store/apps/details?id=com.willhauck.linconnectclient


Windows Server 
---------------

Same application for windows 

https://github.com/vikas0380/linconnect-windows

