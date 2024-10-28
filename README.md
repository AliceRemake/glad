# CMake For GLAD

## Description

this is a cmake project for [glad](https://gen.glad.sh/)

this is a part of [FireEngine](https://github.com/AliceRemake/FireEngine)

## Version

* Generator: `C/C++`
* APIs:
  * `Vulkan Version 1.3`
  * `OpenGL Version 4.6`
  * `OpenGL ES 2 Version 3.2`
  * `GLX Version 1.4`
  * `EGL Version 1.5`
  * `WGL Version 1.0`
* Profile:
  * `Core`
* Extensions:
  * None
* Options
  * [X] alias     Enables function pointer aliasing
  * [ ] debug     debugEnables generation of a debug build
  * [X] header    only  header onlyGenerate a header only version of glad
  * [X] loader    loaderInclude internal loaders for APIs
  * [ ] merge     mergeMerge multiple APIs of the same specification into one file.
  * [X] mx        mxEnables support for multiple GL contexts
  * [ ] on demand On-demand function pointer loading, initialize on use (experimental)


you can also generate by yourself here: https://gen.glad.sh/

## Usage

add in your `CMakeLists.txt`

```cmake
ADD_SUBDIRECTORY(glad)
```

link to your own project

```cmake
TARGET_LINK_LIBRARIES(<your target> PUBLIC GLAD)
```
