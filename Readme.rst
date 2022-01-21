Open Source Brain status tracker
--------------------------------

Sources for the OSB infrastructure status tracker at https://status.opensourcebrain.org.

Adapted from the Fedora community infrastructure status tracker at: https://github.com/fedora-infra/statusfpo

Usage
=====

This uses the `Pelican <https://getpelican.org>`__ static site generator, written in Python.
You can install it using your operating system's package manager, or using `pip` in a virtual environment.

Please see the Makefile for usage.
To create a new on-going outage, you can use:

.. code::

    make ongoingoutage NAME="Outage description"

To create a new planned outage, you can use:

.. code::

    make plannedoutage NAME="Outage description"

When an outage is over, move the post file to the `resolved/` folder, and update the completion date and any other information.
