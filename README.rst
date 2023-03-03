====================
Quick start Appollo
====================

A little project to discover `Appollo <https://appollo.readthedocs.io/en/master/index.html>`_.

-------------
Prerequisites
-------------
For Appollo to work you will need : 

* `Python <https://www.python.org/downloads/>`_ 3.6 or higher.
* `PIP <https://pypi.org/project/pip/>`_.
* An `Apple Developer Account <https://developer.apple.com>`_.
* Spice-Space's `client <https://www.spice-space.org/download.html>`_.

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

After create your application you receive the key linked with it (you will need in the second section)

-----------
First start
-----------

to Retrieve the project :  

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

* **url** and **connection_password** for spice connection
* **user** and **user_password** on remote desktop 

.. warning::  When the build is succeeded the remote desktop is usable during 30'

Now you can launch your software, it is named RemoteViewer on your computer, with the url and connection_password to connect to the remote desktop.

|

When your are logged on remote desktop, follow these 4 easy steps :

1. Open Xcode
2. Select Open an existing project
3. Select file Documents/app/ios/Runner.xcworkspace
4. Enjoy your application

 
-------------
Documentation
-------------

If you want complet documentation or learn more about Appollo, I invite you to visit the `Appllo documentation <https://appollo.readthedocs.io/en/master/index.html#>`_
