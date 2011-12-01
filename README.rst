DBGp client for Vim
===================

This Vim plugin allows to remotely debug using a dbgp compatible debugger, as
xdebug, it has be only tested with XDebug + PHP, but it may work with
other debuggers and languages.

Installation
--------------

Copy ``debugger.py`` and ``debugger.vim`` to your vim plugins directory.


Quick start
------------

Open Vim, press F5 and start your debugger


Configuration
--------------

There are some variables that you can configure in Vim:

``g:debuggerPort`` [9000]
    The port that the plugin will use to receive the connections from the
    debugger

``g:debuggerProxyPort`` [localhost]
    Host where the proxy is

``g:debuggerProxyPort``
    Port used to connect to the proxy, leave it unset if not using proxy

``g:debuggerProxyKey``
    Key used in the connection with the proxy

``g:debuggerMaxChildren`` [32]
    TODO

``g:debuggerMaxData`` [32]
    TODO

``g:debuggerMaxChildren`` [1024]
    TODO

``g:debuggerMaxDepth`` [1]
    Maximum depth level when dumping variables

``g:debuggerMiniBufExpl`` [0]
    TODO

``g:debuggerFileMapping`` [[]]
    Array with pairs of regular expressions to match and replacement strings, e,g:
    ``[['/var/www/[^/]+/(.*)', '/home/' . $USER . '/project/\\1']]``

Usage
------

TODO

More info
----------

* `GDBp protocol definition <http://xdebug.org/docs-dbgp.php>`_
