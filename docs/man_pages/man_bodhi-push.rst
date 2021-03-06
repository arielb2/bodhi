===================
bodhi-push man page
===================

Synopsis
========

``bodhi-push`` [OPTIONS]


Description
===========

``bodhi-push`` is used to select which packages to push out to the mirror network. It has various
flags that can be used to select the package set, and then it emits a fedmsg with the list of
packages to be mirrored.


Options
=======

``--help``

    Show help text and exit.

``--builds TEXT``

    A comma-separated list of builds to include in the push.

``--cert-prefix TEXT``

    The prefix of a fedmsg cert used to sign the message.

``--releases TEXT``

    A comma-separated list of releases to include in this push. By default, current and pending
    releases are selected.

``--request TEXT``

    Push updates for the specified request. Defaults to testing,stable.

``--resume``

    Resume one or more previously failed pushes.

``--staging``

    Use the staging bodhi instance instead of the production instance.

``--username TEXT``

    Your FAS user id.

``--version``

    Show version and exit.


Bugs
====

If you find bugs in bodhi (or in the mage page), please feel free to file a bug report or a pull
request::

    https://github.com/fedora-infra/bodhi
