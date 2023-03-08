====================
Quick start Appollo
====================
Below you will find a quick start project to discorver `Appollo <https://github.com/Appollo-CLI/Appollo>`_. The flutter project in the repository is the project exemple, the flutter counter.

-------------
Prerequisites
-------------
For Appollo to work you will need : 

* `Python <https://www.python.org/downloads/>`_ 3.6 or higher.
* `PIP <https://pypi.org/project/pip/>`_.
* An `Apple Developer Account <https://developer.apple.com>`_.
* A VNC viewer or `RustDesk <https://rustdesk.com/>`_

-----------------
Appollo's install
-----------------
To install appollo run this command :  

.. code-block:: sh

    pip install appollo

|

.. note:: Once installed we can easily run the CLI in the terminal ``appollo`` and you should get the ``help`` output of the terminal.

|

If it is your first time using Appollo, create an Appollo account by running :  

.. code-block:: sh

    appollo signup

|

Link your developer account to Appollo, you will need your team ID, Issuer ID, key ID, and API key file

.. code-block:: sh

    appollo apple add --apple-id TEXT --name TEXT --key-id TEXT --issuer-id TEXT --private-key FILE

|

When the linking is done you receive the Appollo Key

Create an app identifier

.. code-block:: sh

    appollo app mk

|

After create your application you receive the KEY linked with it (you will need in the second section)

-----------
First start
-----------

To retrieve the project

.. code-block:: sh

    git clone https://github.com/NathanSepul/Tutorial-Appollo.git

|

Place you at the root of flutter folder ``tutoral_appollo`` and, if it not already done, connect you to appollo.

.. code-block:: sh

    appollo signin

|

When it is done you can launch the configuration build and select your project

.. code-block:: sh

    appollo build start --build-type configuration APPLICATION_KEY

If your buid has succeeded your receive connection settings and credentials for the remote connection with Spice

* **RustDesk relay server**, **RustDesk ID** and **RustDesk password**

* **VNV url** 

* **user** and **user_password** for the remote desktop 

|

.. warning::  When the build is succeeded the remote desktop is usable during 1hour

Now you can launch your vnc viewer or RustDesk, if you use RustDesk don't forget change the relay server.

|

When your are logged on remote desktop, follow these 4 easy steps :

1. Open Xcode
2. Select Open an existing project
3. Select file Documents/app/ios/Runner.xcworkspace
4. Enjoy your application

|

To test your flutter app in iOS simulator on de the remote desktop place you in application folder with the terminal

.. code-block:: sh

    cd ~/Documents/app

|

and lauch the flutter run command

.. code-block:: sh

    flutter run


-------------
Documentation
-------------

If you want complet documentation or learn more about Appollo, I invite you to visit the `Appllo documentation <https://appollo.readthedocs.io/en/master/index.html#>`_
