**_WARNING_: The AI Programming Final HW is renamed to [rivertensor](https://github.com/RiverHamster/rivertensor), with scikit-build, autodiff and more. This repo is in public archive.**

# PKU Programming in AI class project
This library implements basic NN operators, including matrix multiplication,
2D convolution, pooling, activation functions and loss functions in CUDA C++
and exports a Python binding. It is part of the class project of
[PKU Programming in AI](https://pkuprogramminginai.github.io/Labs-Documentation/#/)
course.

The current status of the project is HW3.

## Building the project
The project is tested on Linux with CUDA 12.3, Python 3.12.7, and pytest 8.3.3.
No Python packaging with `setup.py` is done, and the project is built with CMake.
Make sure `pytest` and `pybind11` is installed with conda to proceed with
building and testing the project.

To build and test the project, use
```bash
./build.sh
pytest test
```

To test the MNIST training, use
```bash
python mnist/mnist.py
```
(You may need to export environment variable `PYTHONPATH=build` in order to find
the Python package, if not done automatically by `.env`)
