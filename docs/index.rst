Overview
--------
Cohen is a DLNA/UPnP Media Server written in Python,
providing several UPnP MediaServers and MediaRenderers
to make simple publishing and streaming different types of media content to your network.

Cohen is actually a highly simplified and refreshed version of
`Coherence Framework <https://github.com/coherence-project/Coherence>`_ project by `Frank Scholz <mailto:dev@coherence-project.org>`_
which looks like no longer supported.

- Latest release: |version| (:ref:`changelog`)
- GitHub: https://github.com/unintended/Cohen
- Issue tracker: https://github.com/unintended/Cohen/issues
- PyPI: https://pypi.python.org/pypi/cohen
- Free software: MIT licence


Features
--------
Cohen is known to work with various clients
    - Sony Playstation 3/4
    - XBox360/One
    - Denon AV Receivers
    - WD HD Live MediaPlayers
    - Samsung TVs
    - Sony Bravia TVs

And provides a lot of backends to fulfil your media streaming needs
    - Local file storage
    - YouTube
    - Twitch.tv
    - and much more...

Quickstart
----------
To just export some files on your hard-disk fire up Cohen with
an UPnP MediaServer with a file-system backend enabled::

  $ cohen --plugin=backend:FSStore,content:/path/to/your/media/files

You can also configure cohen via a config file. Feel free to check our example ``misc/cohen.conf.example``.
The config file can be placed anywhere, cohen looks by default for
``$HOME/.cohen``, but you can pass the path via the commandline option
'-c' to it too::

  $ cohen -c /path/to/config/file


Table of Contents
-----------------

.. toctree::
    :glob:

    install
    cli
    backends
    backend/*
