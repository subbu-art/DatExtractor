dateutil - powerful extensions to datetime
==========================================

|pypi| |support| |licence|

|gitter| |readthedocs|

|travis| |appveyor| |pipelines| |coverage|

.. |pypi| image:: https://img.shields.io/pypi/v/python-dateutil.svg?style=flat-square
    :target: python link
    :alt: pypi version

.. |support| image:: https://img.shields.io/pypi/pyversions/python-dateutil.svg?style=flat-square
    :target: 
    :alt: supported Python version

.. |licence| image:: https://img.shields.io/pypi/l/python-dateutil.svg?style=flat-square
    :target: 
    :alt: licence

.. |readthedocs| image:: https://img.shields.io/readthedocs/dateutil/latest.svg?style=flat-square&label=Read%20the%20Docs
   :alt: Read the documentation at https://dateutil.readthedocs.io/en/latest/
   :target: https://dateutil.readthedocs.io/en/latest/

The `DatExtractor` module provides the most efficient way of 
extracting date from text, available in Python.

Installation
============
`DatExtractor` can be installed from PyPI using `pip` (note that the package 
name is different from the importable name)::

    pip install DatExtractor

Download
========
dateutil is available on PyPI
https://pypi.org/project/python-dateutil/

The documentation is hosted at:
https://dateutil.readthedocs.io/en/stable/

Code
====
The code and issue tracker are hosted on GitHub:
https://github.com/dateutil/dateutil/

Features
========

* This Package help you to extract date from the text.
* You can get the date in what ever format you actually want it.
* Currently the package can handle formats seperated by [/.-]. 
* Generic parsing of dates in almost any string format.
* You can extract multiple dates as well and you can use it as per the requirement.

Quick example
=============
Here's a snapshot, just to give an idea about the power of the
package. For more examples, look at the documentation.

Suppose you want to extract date from a text. you need to provide the 
text to the function as an argument. the default format of 
date you get is (mm/dd/yyyy). However you can modify the date format by 
passing the date format argument, so that you get the date in expected format.:

.. doctest:: readmeexample

    >>> from DatExtractor import date_parser
    >>> date_parser("Please find the status of the following invoice 4063979243 on date:- 29/10/2020 with PO number:- 1548546745")
    ['10/29/2020']
    >>> date_parser("Please find the status of the following invoice 4063979243 on date:- 29/10/2020 with PO number:- 1548546745","%Y/%d/%m")
    ['2020/29/10']
    >>> date_parser("Please find the status of the following invoice 4063979243 on date:- 29/10/2020 with PO number:- 1548546745","%d/%Y/%m")
    ['29/2020/10']


Author
======
The DatExtractor module was written by Sri Phani Subramanyam <subbu27498@gmail.com> in 2021.

It is maintained by:

* Sri Phani Subramanyam <subbu27498@gmail.com> 2021-Present
  
Contact
=======
For queries please contact <subbu27498@gmail.com>. 

License
=======

Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
Everyone is permitted to copy and distribute verbatim copies
of this license document, but changing it is not allowed. `GNU General Public License v3.0 <https://choosealicense.com/licenses/gpl-3.0/#>`.