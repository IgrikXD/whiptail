====================
whiptail-dialogs
====================

.. start short_desc

**Use whiptail to display dialog boxes from Python scripts.**

.. end short_desc

.. start shields

.. list-table::
	:stub-columns: 1
	:widths: 10 90

	* - Info
	  - |docs| |requires| |commits-latest|

.. |docs| image:: https://img.shields.io/readthedocs/whiptail/latest?logo=read-the-docs
	:target: https://whiptail.readthedocs.io/en/latest
	:alt: Documentation Build Status

.. |requires| image:: https://dependency-dash.repo-helper.uk/github/IgrikXD/whiptail-dialogs/badge.svg
	:target: https://dependency-dash.repo-helper.uk/github/IgrikXD/whiptail-dialogs/
	:alt: Requirements Status

.. |commits-latest| image:: https://img.shields.io/github/last-commit/IgrikXD/whiptail-dialogs
	:target: https://github.com/IgrikXD/whiptail-dialogs/commit/master
	:alt: GitHub last commit

.. end shields


``whiptail`` is a library that will let you present a variety of questions or
display messages using dialog boxes from a Python script.

Currently, these types of dialog boxes are implemented:

* yes/no box
* menu box
* input box
* message box
* text box
* info box
* checklist box
* radiolist box
* gauge box
* password box

Differences from the original project
--------------
Now, when calling **msgbox()**, you can specify additional options by specifying them in the **extra_args** variable. For example:

.. code-block:: python

	w = Whiptail(title="This is the title", backtitle="This is the backtitle")
	w.msgbox("This is a msgbox!", extra_args=["--scrolltext"])

Now, when calling **menu()** and **showlist()**, multi-line messages will be processed correctly. Previously, you would lose part of a message if it was more than two lines high.

Installation
--------------

.. start installation

``whiptail`` can be installed from PyPI.

To install with ``pip``:

.. code-block:: bash

	$ pip install git+https://github.com/IgrikXD/whiptail-dialogs@master

.. end installation

You must also have the ``whiptail`` package installed on your system.

On Debian and derivatives this can be installed with:

.. code-block:: bash

	$ sudo apt install whiptail
