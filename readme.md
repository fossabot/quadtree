# Quadtrees iterating on pairs of neighbours
[![FOSSA Status](https://app.fossa.com/api/projects/git%2Bgithub.com%2Fdhanesh123in%2Fquadtree.svg?type=shield)](https://app.fossa.com/projects/git%2Bgithub.com%2Fdhanesh123in%2Fquadtree?ref=badge_shield)


Implementation of a smart version of quadtrees specialised in tracking distance
between moving objects.

## Python interface

### Installation

Recommended installation procedure :
- `virtualenv` (optional, but a good idea nonetheless):
```
 virtualenv quadtree_test
 source quadtree_test/bin/activate
```
- installation:
```
pip install smartquadtree
```

If no version is available, you can compile your own:
```
pip install git+git://github.com/xoolive/quadtree
```

### Usage

```python
import smartquadtree
```

You can refer to the `tutorial.iypnb` file for an introduction to the
possibilities of the package. If you are not familiar with the iPython
notebook, you can also access to a static version on [PyPI](https://pypi.python.org/pypi/smartquadtree)

## C++ library

### Installation

You can use CMake to build the C++ library.

The minimal installation is obtained by setting the `BUILD_TESTS`
option to `OFF`. If you keep the `BUILD_TESTS` option `ON`, you will
need to have OpenGL and GLUT installed. `freeglut` is a valid
implementation for the current example.

If you try the library in a virtual machine, **do** set the `RUN_IN_VM`
option to `ON`.

You can try the application by launching `make run`. The simulation is
made of elements moving in a map. A red line is drawn between elements
closer than a preset threshold. At the beginning of the simulation, all
elements inside a predefined shape are painted in green.

You can then:
 - zoom in/out with `+`/`-`;
 - move left/down/up/right with the standard vim movement keys: `h`, `j`, `k`, `l`;
 - press `g` to repaint elements inside the original shape in green. 

### Usage

A good way to learn how to use the library would be to have a look at
file `tests/test_simu.cpp`.

For a more basic introduction, it is recommended to start with the
Python interface, its documentation, and the `tutorial.ipynb` file that
you can also view 
[here](http://nbviewer.ipython.org/github/xoolive/quadtree/blob/master/tutorial.ipynb).


## License
[![FOSSA Status](https://app.fossa.com/api/projects/git%2Bgithub.com%2Fdhanesh123in%2Fquadtree.svg?type=large)](https://app.fossa.com/projects/git%2Bgithub.com%2Fdhanesh123in%2Fquadtree?ref=badge_large)