====
mova
====

mova - Multi-homed Nova command-line client wrapper

Description
===========

``mova`` is a very lightweight wrapper around `nova
<https://github.com/openstack/python-novaclient>`_ that allows you to work
with multiple environments.

mova serves the same purpose as the excellent `supernova
<https://github.com/major/supernova>`_ utility, but differs in a few key ways.

Features
========

- **Stateful**: You don't have to specify the environment for each command, just
  specify it once each time you change environments
- **Tab-completion**: Nova's tab-completion still works
- **Standard**: Uses Nova's standard ``novarc`` files, just place them in ``~/.mova/`` with
  descriptive names like 'prod' and 'dev'
- **Simple**: Single bash file


Setup
=====

- Add ``mova`` to your ``bashrc``
- Create ``~/.mova`` directory
- Copy existing ``novarc`` files into it, giving them descriptive file names


List Available Environments
===========================

::

    $ mova
    dev
    lab
    prod (current)


Change Current Environment
==========================

::

    $ mova use dev


Run Nova Command Under Current Environment
==========================================

::

    $ mova list
    $ mova image-list


Author
======

Rick Harris
