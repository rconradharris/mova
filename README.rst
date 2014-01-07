===================================================
mova - Multi-homed Nova command-line client wrapper
===================================================

Description
===========

`mova` is a very lightweight wrapper around `nova` that allows you to work
with multiple environments.

Features
========

- Stateful: You don't have to specify the environment for each command, just
  specify it once each time you change environments
- Tab-completion: Nova's tab-completion still works
- Uses Nova's standard `novarc` files, just place them in ~/.mova/ with
  descriptive names like 'prod' and 'dev'
- Single bash file


Setup
=====

- Create ~/.mova directory
- Copy existing `novarc` files into it, giving them descriptive file names
- Source `mova` or add it to your `bashrc`


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
