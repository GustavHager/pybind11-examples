# Example of how to get pybind11 to work

Just a simple example of how to get pybind11 [1] to work with C++ and numpy.

This repository includes the pybind11 code as a submodule, it must be initialized after cloning the repository.

```bash
git submodule update --init --recursive
```

before it can be compiled

## Requirements for ubuntu 18.04:
python3-dev
cmake


# Help, it does not work!
* The module name must match in cmake and in the c++ file
* you need to move or symlink the compiled .so files from the build directory to the python directory for python to find them correctly

[1] https://github.com/pybind/pybind11
