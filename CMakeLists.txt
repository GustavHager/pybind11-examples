cmake_minimum_required(VERSION 3.0)
project(pybind11_examples)

# Add the submodule
add_subdirectory(dependencies/pybind11)

# Tell the pybind11 system to do its magic on the python module called "example_functions"
# found in the file functions.cpp
# EXTREMELY IMPORTANT THAT THE MODULE NAMES MATCH IN BOTH PLACES
pybind11_add_module(example_functions src/functions.cpp)
