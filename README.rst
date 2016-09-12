$4810Vision
===========

4810Vision is an implementation of OpenCV in order to detect targets for the 2016 FRC Competition Game, "Stronghold." The code is written in Python 3+


Features
--------

- A direct implementation of the FRC 2016 Vision Tutorial. Read more here_.
- Relative accuracy in detecting the high goals in "Stronghold"
- A folder of sample pictures to showcase said accuracy


.. _here: https://wpilib.screenstepslive.com/s/4485/m/24194/l/288985-identifying-and-processing-the-targets

Usage
-----

Usage is fairly simple. Simply clone the repository into your directory and run the Python code that is required. That is as simple as

.. highlight:: console
	       
   python3 vision.py

.. highlight:: none

Installation
------------

This is to be done *before* usage and can be quite a tedious process. First you'll need to settle on an operating system.

If it's Windows, follow these steps (make sure to have admin privileges, when needed)

1) Download Python 3.4+, which can be found at http://python.org. You'll need to set it up in $PATH as an environment variable to be able to use it in the command line.
2) When you download Python 3.4+, you should have a working version of pip, which will be needed to grab some required libraries built for Python to have OpenCV working. To ensure that it Python recognizes pip, run

.. highlight:: powershell


   pip

.. highlight:: none

in your command shell. If that is not the case, then download pip from the official website. Download the Python file get-pip.py and then simply run it with Python.
3) We will now grab the dependencies that OpenCV needs to work on pip, namely numpy and matplotlib (the latter is moreso optional but very helpful). Simply run
.. highlight:: powershell

   pip install numpy
   pip install matplotlib

.. highlight:: none

and pip should take care of the rest.
4) Now for the most exciting part: actually getting OpenCV. For Windows, we are getting a precompiled binary for opencv3. To do so head over to this website
   http://www.lfd.uci.edu/~gohike/pythonlibs/
Find opencv on the list of Python Extension Packages (there's a lot) and click on the link. This should take you to a bynch of .whl files to download. Make sure you grab the .whl file that
   - Corresponds to your version of Python 3 (3.4 or 3.5 are both supported)
   - Matches your system architecture (32 or 64 bit)
Download and then run
.. highlight:: powershell


   pip install opencv_python-3.1.0-cp3x-cp3xm-architecturehere.whl

.. highlight:: none
This should install opencv for use in Python
5) Now we sit back and test to see if it works. To do so run Python in command line and invoke the following commands
.. highlight:: python

   import cv2
   cv2.__version__

.. highlight:: none
If you get no errors, then you are all set!
Happy editing.
