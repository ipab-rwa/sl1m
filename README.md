# sl1m

[![Pipeline status](https://gitlab.laas.fr/$ORG/sl1m/badges/master/pipeline.svg)](https://gitlab.laas.fr/loco-3d/sl1m/commits/master)
[![Coverage report](https://gitlab.laas.fr/loco-3d/sl1m/badges/master/coverage.svg?job=doc-coverage)](http://projects.laas.fr/gepetto/doc/loco-3d/sl1m/master/coverage/)


## Python dependencies:
- scipy
- quadprog
- matplotlib
- pycddlib
- cvxpy

:warning: this package optionally requires gurobi :warning:
A free academic license can be obtained at https://www.gurobi.com
Otherwise the Mixed Integer formulation provded by COIN-OR can be used through the cvxpy interface (but it is quite slow)


## Installation:
After cloning the repository, initialise the submodules, build and install the library
```bash
git submodule update --init
mkdir build && cd build && cmake ..  -DCMAKE_BUILD_TYPE=Release   -DCMAKE_POLICY_VERSION_MINIMUM=3.5  
make
make install
```
