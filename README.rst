Introduction
============




.. image:: https://img.shields.io/discord/327254708534116352.svg
    :target: https://adafru.it/discord
    :alt: Discord


.. image:: https://github.com/CedarGroveStudios/CircuitPython_TouchCalibrator/workflows/Build%20CI/badge.svg
    :target: https://github.com/CedarGroveStudios/CircuitPython_TouchCalibrator/actions
    :alt: Build Status


.. image:: https://img.shields.io/badge/code%20style-black-000000.svg
    :target: https://github.com/psf/black
    :alt: Code Style: Black

A simple CircuitPython DisplayIO resistive touchscreen calibrator for Adafruit
built-in and TFT FeatherWing displays.

On-screen touchscreen calibrator for built-in and TFT FeatherWing displays. To
use, run as a standalone module, include the following line in the calling
module, or type into the REPL:

.. code-block:: python

       import touchcalibrator.built_in

for built-in displays or

.. code-block:: python

       import touchcalibrator.featherwing

for TFT FeatherWing displays.

Operational parameters such as screen rotation and REPL-only measurement display
can be set in the ``operational parameters`` portion of the module.

When the test screen appears, use a stylus to swipe to the four edges of the
visible display area. As the screen is calibrated, the small red square tracks
the stylus tip (when ``REPL_ONLY=False``). Minimum and maximum calibration
values will display on the screen and in the REPL. The REPL values can be copied
and pasted into the calling code's touchscreen instantiation statement.

Touchscreen Instantiation example code for built-in displays.
The order of the calibration tuples is determined by the display rotation value:

.. image: https://github.com/CedarGroveStudios/CircuitPython_TouchCalibrator/blob/main/media/Touch_Calib_example.png
    :alt: Touchscreen Instantiation Example Code

.. image: https://github.com/CedarGroveStudios/CircuitPython_TouchCalibrator/blob/main/media/touch_calibrator_screen.jpg)
    :alt: Screen Image Example


Dependencies
=============
This driver depends on:

* `Adafruit CircuitPython <https://github.com/adafruit/circuitpython>`_

Please ensure all dependencies are available on the CircuitPython filesystem.
This is easily achieved by downloading
`the Adafruit library and driver bundle <https://circuitpython.org/libraries>`_
or individual libraries can be installed using
`circup <https://github.com/adafruit/circup>`_.

Installing to a Connected CircuitPython Device with Circup
==========================================================

Make sure that you have ``circup`` installed in your Python environment.
Install it with the following command if necessary:

.. code-block:: shell

    pip3 install circup

With ``circup`` installed and your CircuitPython device connected use the
following command to install:

.. code-block:: shell

    circup install cedargrove_touchcalibrator

Or the following command to update an existing version:

.. code-block:: shell

    circup update

Usage Example
=============

.. todo:: Add a quick, simple example. It and other examples should live in the
examples folder and be included in docs/examples.rst.

Documentation
=============
API documentation for this library can be found on `Read the Docs <https://circuitpython-touchcalibrator.readthedocs.io/>`_.

For information on building library documentation, please check out
`this guide <https://learn.adafruit.com/creating-and-sharing-a-circuitpython-library/sharing-our-docs-on-readthedocs#sphinx-5-1>`_.

Contributing
============

Contributions are welcome! Please read our `Code of Conduct
<https://github.com/CedarGroveStudios/Cedargrove_CircuitPython_TouchCalibrator/blob/HEAD/CODE_OF_CONDUCT.md>`_
before contributing to help this project stay welcoming.
