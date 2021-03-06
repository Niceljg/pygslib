PyGSLIB
=======

Version:  '0.0.0.4.0.0'  
Documentation: https://opengeostat.github.io/pygslib/   
Wiki: https://github.com/opengeostat/pygslib/wiki   
Source code: https://github.com/opengeostat/pygslib   
Videos: https://www.youtube.com/c/opengeostat   

This is an open source python module for mineral resource estimation and geostatistics. It consists of:  

- ``gslib``. This is for geostatistics and interpolation. It was built with
 [GSLIB Fortran 77 code] (http://www.statios.com/Quick/gslib.html) enhanced and
 wrapped to Python with [f2py](http://docs.scipy.org/doc/numpy-dev/f2py/).
- ``drillhole``. This is for basic drillhole operations, such as compositing and desurveying.
- ``blockmodel``. This is for block modelling, it has functions to fill wireframes
 with blocks, reblocking, among others.
- ``vtktools``. This is for 3D computational geometry based on VTK, for example,
 to select samples within wireframes. It also handles VTK files.
- ``nonlinear``. This module is under construction! It is an experimental module
 for nonlinear geostatistics based on the Discrete Gaussian Model.
- `sandbox` Here we put general code and testing code.

Installation in Anaconda/Miniconda distributions (Linux, Window and OS)
------------
The easiest way to install and work with PyGSLIB is using Anaconda or Miniconda (conda) distributions. To install PyGSLIB in the root environment of your anaconda distribution simply type in a terminal:  

```
$ conda install pygslib -c opengeostat -c conda-forge
```

Installation from source (from github.com)
--------------------
This is the most update but unstable development version. You may manually
install all the dependencies and make sure you have gfortran available.  

Windows users may read [this wiki](https://github.com/opengeostat/pygslib/wiki/Before-compiling-in-Windows) first. It explains how to prepare the development environment (compilers and dependencies).

```
$ git clone https://github.com/opengeostat/pygslib.git
$ cd pygslib
$ python setup.py build
$ python setup.py install
```

Usage
-----
See this [tutorial] (https://opengeostat.github.io/pygslib/Tutorial.html). There is also a [video demonstration]( https://youtu.be/SEwKy6wJbLE) that uses  
an older version of pygslib.

License
-------
Copyright 2018, Adrian Martinez Vargas

This software may be modified and distributed under the terms of the
[MIT](https://github.com/opengeostat/pygslib/blob/master/LICENSE.txt) and [GPL](https://www.gnu.org/licenses/gpl-3.0.en.html) licenses.  

Sunday, 19 of August 2018
