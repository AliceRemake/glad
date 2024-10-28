# CMake For GLAD

## Description

this is a cmake project for [glad](https://glad.dav1d.de/)

this is a part of [FireEngine](https://github.com/AliceRemake/FireEngine)

## Version

* Language: `C/C++`
* Specification: `OpenGL`
* API:
  * gl: `Version 4.6`
  * gles1: `None`
  * gles2: `None`
  * glcs2: `None`
  * Profile: `Core`
* Extensions:
  * empty

you can generate yourself here: https://glad.dav1d.de/

## Usage

add in your `CMakeLists.txt`

```cmake
ADD_SUBDIRECTORY(glad)
```

link to your own project

```cmake
TARGET_LINK_LIBRARIES(<your target> PUBLIC GLAD_STATIC)
# or
TARGET_LINK_LIBRARIES(<your target> PUBLIC GLAD_SHARED)
```

## Stand-Alone Build

```bash
mkdir build && cd build
cmake ..
make -j16
```
