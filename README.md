# Simple simdutf demo for vcpkg
[![Linux-CI](https://github.com/simdutf/simdutf-vcpkg/actions/workflows/linux.yml/badge.svg)](https://github.com/simdutf/simdutf-vcpkg/actions/workflows/linux.yml)
[![Windows-CI](https://github.com/simdutf/simdutf-vcpkg/actions/workflows/ci.yml/badge.svg)](https://github.com/simdutf/simdutf-vcpkg/actions/workflows/ci.yml)

This project builds a simple executable that
depends on simdutf, under Windows and Linux. 

After installing vcpkg and installing
simdutf through it (e.g., `vcpkg install simdutf:x64-windows` or `vcpkg install simdutf`), you can build with CMake using a couple of command lines.

You need to pass the location of your `vcpkg/scripts/buildsystems/vcpkg.cmake`  file to CMake:

```
cmake -DCMAKE_TOOLCHAIN_FILE=<location> -B build
cmake --build build
```
