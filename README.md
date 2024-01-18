# Introduction

This is the new SDK for Arducam EVK, currently in beta version and supports Linux and Windows.

## API documentation

For detailed API reference and usage instructions,
please refer to the [Arducam online documentation](https://www.arducam.com/docs/arducam-evk/).

## Installation dependence
### Linux
please refer to the [linux install opencv Driver](doc/linux_install_opencv_Driver.md)

### Windows
please refer to the [windows install opencv Driver](doc/linux_install_opencv_Driver.md)

## What's next
The project contains multiple demos, please try them according to the corresponding descriptions.
```
    .
    ├── c                           # C Demo
    │   ├── COption.cmake           # C Demo CMake compilation parameter settings and import
    │   ├── functions               # C Demo source code (independent use cases for each function)
    │   └── projects                # C Demo project (integration use cases of common functions)
    │       ├── FindOpenCV.cmake    # CMake looking for OpenCV library
    │       ├── simple              # Simple synchronous collection Demo
    │       ├── simple-async        # Simple asynchronous collection Demo
    │       ├── sync                # Synchronous collection of Demo
    │       └── async               # Asynchronous collection Demo
    ├── c++                         # C++ Demo
    │   ├── CppOption.cmake         # C++ Demo CMake compile parameter settings and import arducam_evk_cpp_sdk
    │   ├── functions               # C++ Demo source code (independent use cases for each function)
    │   └── projects                # C++ Demo project (integration use cases of common functions)
    │       ├── FindOpenCV.cmake    # CMake looking for OpenCV library
    │       ├── sync                # Synchronous collection of Demo
    │       └── async               # Asynchronous collection Demo
    ├── python                      # Python Demo
    │   ├── requirements.txt        # python demo dependent libraries
    │   ├── README.md               # python demo introduction and usage
    │   ├── function                # python demo source code (independent use cases for each function)
    │   └── project                 # python demo project (integrated use cases for common functions)
    │       ├── utils.py            # Project tool function
    │       ├── sync.py             # Synchronous collection of Demo
    │       └── async.py            # Asynchronous collection Demo
    └── README.md                   
```
