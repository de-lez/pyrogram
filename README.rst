|header|

Table of Contents
=================

-   `About`_

    -   `Features`_

    -   `Requirements`_

-   `Getting Started`_
    
    -   `Installation`_
    
    -   `Configuration`_
    
    -   `Usage`_

-   `Documentation`_

-   `Contribution`_

-   `Feedback`_

-   `License`_


About
=====

**Pyrogram** is a brand new Python library for building custom `Telegram`_ clients. It can be used
to interact with Telegram via the MTProto API as both User and Bot and to execute any action an official
app is able to do (and more).

Features
--------

``Pyrogram`` has many advantages over other libraries:

-   **Easy to setup**: ``Pyrogram`` can be easily installed using pip and requires very few lines of code to
    get started with.

-   **Easy to use**: ``Pyrogram`` provides idiomatic, developer-friendly, clean and readable Python code making
    the Telegram API simple to use.

-   **High-level**: ``Pyrogram`` automatically handles all the low-level details of communication with
    Telegram servers.

-   **Fast**: ``Pyrogram`` speed is boosted up by `TgCrypto`_, a high-performance Telegram Crypto Library
    written in C.

-   **Updated**: ``Pyrogram`` makes use of the latest Telegram MTProto API version.

-   **Documented**: ``Pyrogram`` API methods are documented and resemble the well established Telegram Bot API,
    thus offering a familiar look to Bot developers.

-   **Full API support**: Beside the simple, Bot API-like methods, ``Pyrogram`` also provides a complete access
    to every single Telegram MTProto API method.


Requirements
------------

-   Python 3.3 or higher.

-   A Telegram API key.
    

Getting Started
===============

Installation
------------

-   You can easily install and upgrade the library using standard Python tools:

    .. code:: shell

        $ pip3 install --upgrade pyrogram
        
-   Or, with TgCrypto_:

    .. code:: shell

        $ pip3 install --upgrade pyrogram[tgcrypto]

Configuration
-------------

-   Create a new ``config.ini`` file at the root of your working directory, copy-paste
    the following and replace the **api_id** and **api_hash** values with `your own`_:

    .. code:: ini

        [pyrogram]
        api_id = 12345
        api_hash = 0123456789abcdef0123456789abcdef

Usage
-----

-   And here's how ``Pyrogram`` looks like:

    .. code:: python

        from pyrogram import Client

        client = Client("example")
        client.start()

        client.send_message("me", "Hi there! I'm using Pyrogram")
        client.send_photo("me", "/home/dan/pic.jpg", "Nice photo!")

        client.stop()
    
That's all you need for getting started with ``Pyrogram``. For more detailed information,
please refer to the Documentation_.


Documentation
=============

- The entire ``Pyrogram`` documentation resides at https://docs.pyrogram.ml.


Contribution
============

**You are very welcome to contribute** by either submitting pull requests or
reporting issues/bugs as well as suggesting best practices, ideas, enhancements
on both code and documentation. Any help is appreciated!


Feedback
========

Means for getting in touch:

-   `Community`_
-   `GitHub`_
-   `Email`_


License
=======

-   Copyright (C) 2017-2018 Dan Tès <https://github.com/delivrance>

-   Licensed under the terms of the
    `GNU Lesser General Public License v3 or later (LGPLv3+)`_
    

.. _`Telegram`: https://telegram.org/

.. _`your own`: https://docs.pyrogram.ml/start/ProjectSetup/#api-keys

.. _`Community`: https://t.me/PyrogramChat

.. _`bot-like`: https://core.telegram.org/bots/api#available-methods

.. _`GitHub`: https://github.com/pyrogram/pyrogram/issues

.. _`Email`: admin@pyrogram.ml

.. _TgCrypto: https://github.com/pyrogram/tgcrypto

.. _`GNU Lesser General Public License v3 or later (LGPLv3+)`: COPYING.lesser

.. |header| raw:: html

    <h1 align="center">
        <a href="https://pyrogram.ml">
            <div><img src="https://pyrogram.ml/images/icon.png" alt="Pyrogram Icon"></div>
            <div><img src="https://pyrogram.ml/images/label.png" alt="Pyrogram Label"></div>
        </a>
    </h1>

    <p align="center">
        <b>Telegram MTProto API Client Library for Python</b>
        
        <br>
        <a href="https://github.com/pyrogram/pyrogram/releases/latest">
            Download
        </a>
        •
        <a href="https://docs.pyrogram.ml">
            Documentation
        </a>
        •
        <a href="https://t.me/PyrogramChat">
            Community
        </a>
        <br><br>
        <a href="compiler/api/source/main_api.tl">
            <img src="https://www.pyrogram.ml/images/scheme.svg"
                alt="Scheme Layer 75">
        </a>
        <a href="https://github.com/pyrogram/tgcrypto">
            <img src="https://www.pyrogram.ml/images/tgcrypto.svg"
                alt="TgCrypto">
        </a>
    </p>

.. |logo| image:: https://pyrogram.ml/images/logo.png
    :target: https://pyrogram.ml
    :alt: Pyrogram

.. |description| replace:: **Telegram MTProto API Client Library for Python**

.. |scheme| image:: https://www.pyrogram.ml/images/scheme.svg
    :target: compiler/api/source/main_api.tl
    :alt: Scheme Layer 75

.. |tgcrypto| image:: https://www.pyrogram.ml/images/tgcrypto.svg
    :target: https://github.com/pyrogram/tgcrypto
    :alt: TgCrypto
