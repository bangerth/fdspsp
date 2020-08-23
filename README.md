# FDS Particle Spray Postprocessing (fdspsp)

`fdspsp` offers tools to postprocess particle data generated with NIST's [Fire Dynamics Simulator (FDS)](https://github.com/firemodels/fds).

- Read `*.prt5` binary files containing particle data in the FORTRAN format described in the [`FDS 6.7.1` user's guide, section 24.10 particle data](https://github.com/firemodels/fds/releases/download/FDS6.7.1/FDS_User_Guide.pdf).
- Determine the spray front of particle clouds using the following algorithms described in the [`fdspsp` publication](https://www.google.com/).
  - *farthest fraction method (FF)*
  - *grid density method (GD)*
  - *grid coverage method (GC)*
- Plot postprocessed data.

Currently, there is no intention to provide a wiki for this repository.
Please consult the documentation provided by Docstrings and study the examples to get started.


## Installation

`fdspsp` requires [`python3`](https://www.python.org/) along with [`numpy`](https://numpy.org/) for usage and [`setuptools`](https://github.com/pypa/setuptools) during installation.
We recommend using a version of `FDS` more recent than `>= 6.7.1` in combination with `fdspsp`.

Install `fdspsp` by cloning this repository and installing it to your `python3` distribution.
```
$ git clone https://github.com/FireDynamics/fdspsp
$ cd fdspsp
$ python setup.py install
```

You can then import it into your `python` scripts as a module
```
import fdspsp
```
or
```
from fdspsp import *
```


## Publications

This toolbox has been developed to characterize water sprays and fire balls in the following literature.
Please cite the former publication if you use `fdspsp`.

```
@article{fdspsp2020,
  author  = {Marc Fehling and Michael Krampf and Lukas Arnold},
  title   = {? Project fireballs},
  journal = {? Fire Safety Journal},
  volume  = {?},
  issue   = {?},
  year    = {? 2020},
  pages   = {?},
  doi     = {?}
}

@mastersthesis{krampf2018,
  author  = {Michael Krampf},
  title   = {{C}harakterisierung der {L}iftoff {P}hase partikelbasierter {F}euerb{\"a}lle},
  school  = {Univ. Wuppertal},
  pages   = {69 p},
  year    = {2018},
  url     = {https://juser.fz-juelich.de/record/865224}
}
```
