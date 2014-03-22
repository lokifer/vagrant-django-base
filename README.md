vagrant-django-base
===================

A Vagrant box based on Ubuntu precise64, configured for Django 1.6 development.
Modified from torchbox/vagrant-django-base.

* postgresql 9.3 (with locale fixed to create databases as UTF-8)
* virtualenv and virtualenvwrapper
* dependencies for PIL, the Python Imaging Library
* a pip download cache pre-seeded with Django and various other common packages
* git (sometimes required for pip dependencies that aren't in PyPI)
* postgresql user vagrant, db appname, password dev

Build instructions
------------------
To generate the .box file:

    ./build.sh

To install locally:

    vagrant box add django-base-v2 django-base-v2.box
