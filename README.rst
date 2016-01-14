===============================
FDecimal
===============================

.. image:: https://img.shields.io/travis/bennylope/fdecimal.svg
        :target: https://travis-ci.org/bennylope/fdecimal

.. image:: https://img.shields.io/pypi/v/fdecimal.svg
        :target: https://pypi.python.org/pypi/fdecimal


Implicit float-operations compatability for Python Decimal arithmetic.

* Free software: BSD license

Features
--------

Implicit float-to-Decimal coercion for arithmetic operations.

Instead of this::

    >>> from decimal import Decimal
    >>> Decimal(12.0) * 0.5
    TypeError: unsupported operand type(s) for *: 'Decimal' and 'float'

Use FDecimal::

    >>> from fdecimal import FDecimal
    >>> FDecimal(12.0) * 0.5
    FDecimal('6.0')

TODO
----

* Missing operations, including mod, floor div
* Python 3 support
* Allow cdecimal swap-in

Done:

* Return FDecimal objects rather than Decimal objects
