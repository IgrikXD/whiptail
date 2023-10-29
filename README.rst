====================
whiptail
====================

.. start short_desc

**Use whiptail to display dialog boxes from Python scripts.**

.. end short_desc

.. start shields

.. list-table::
	:stub-columns: 1
	:widths: 10 90

	* - Docs
	  - |docs|
	* - PyPI
	  - |pypi-version| |supported-versions| |supported-implementations| |wheel|
	* - Activity
	  - |commits-latest| |commits-since| |maintained| |pypi-downloads|
	* - QA
	  - |codefactor|
	* - Other
	  - |license| |requires|

.. |docs| image:: https://img.shields.io/readthedocs/whiptail/latest?logo=read-the-docs
	:target: https://whiptail.readthedocs.io/en/latest
	:alt: Documentation Build Status

.. |requires| image:: https://dependency-dash.repo-helper.uk/github/IgrikXD/whiptail/badge.svg
	:target: https://dependency-dash.repo-helper.uk/github/IgrikXD/whiptail/
	:alt: Requirements Status

.. |codefactor| image:: https://img.shields.io/codefactor/grade/github/domdfcoding/whiptail?logo=codefactor
	:target: https://www.codefactor.io/repository/github/domdfcoding/whiptail
	:alt: CodeFactor Grade

.. |license| image:: https://img.shields.io/github/license/IgrikXD/whiptail
	:target: https://github.com/IgrikXD/whiptail/blob/master/LICENSE
	:alt: License

.. |commits-since| image:: https://img.shields.io/github/commits-since/domdfcoding/whiptail/v0.4.0
	:target: https://github.com/domdfcoding/whiptail/pulse
	:alt: GitHub commits since tagged version

.. |commits-latest| image:: https://img.shields.io/github/last-commit/IgrikXD/whiptail
	:target: https://github.com/IgrikXD/whiptail/commit/master
	:alt: GitHub last commit

.. |maintained| image:: https://img.shields.io/maintenance/yes/2022
	:alt: Maintenance

.. |pypi-downloads| image:: https://img.shields.io/pypi/dm/whiptail-dialogs
	:target: https://pypi.org/project/whiptail-dialogs/
	:alt: PyPI - Downloads

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

Installation
--------------

.. start installation

``whiptail`` can be installed from PyPI.

To install with ``pip``:

.. code-block:: bash

	$ pip install git+https://github.com/IgrikXD/whiptail@master

.. end installation

You must also have the ``whiptail`` package installed on your system.

On Debian and derivatives this can be installed with:

.. code-block:: bash

	$ sudo apt install whiptail
