Usage
=====

.. _installation:

Installation
------------

To use patm, first install it using pip:

.. code-block:: console

   (.venv) $ pip install patm

Calculate the infrared spectrum of Earth's atmosphere
-----------------------------------------------------

To retrieve a standard earth atmosphere, use the
you can use the ``patm.earth.get_preset_atm("us_standard")`` function:

.. autofunction:: patm.earth.get_preset_atm

The parameter should be either ``"us_standard"``, ``"fish"``,
or ``"veggies"``. Otherwise, :py:func:`patm.earth.get_preset_atm`
will raise an exception.

.. autoexception:: patm.earth.InvalidKindError

For example:

>>> from patm import earth
>>> earth.get_preset_atm("us_standard")

