# Intel(R) Metrics Discovery Application Programming Interface

## Introduction

This software is a user mode library that provides access to GPU performance data.

The library has OS abstraction layer that allows for interoperability in different environments.

## License

Intel(R) Metrics Discovery Application Programming Interface is distributed under the MIT License.

You may obtain a copy of the License at:
https://opensource.org/licenses/MIT

## Supported Platforms

- Intel(R) Processors with Gen9 graphics devices (formerly Skylake, Kaby Lake, Apollo Lake/Broxton, Gemini Lake, Coffee Lake),
- Intel(R) Processors with Gen8 graphics devices (formerly Broadwell),
- Intel(R) Processors with Gen7.5 graphics devices (formerly Haswell).

## Supported Operating Systems

Intel(R) Metrics Discovery Application Programming Interface is supported on Linux family operating systems with minimum kernel version 4.14.

*Exception: for Gen7.5 graphics devices minimum kernel version 4.17 is required*.

## Building

1\. Download sources.

2\. Run CMake generation:

```shell
cmake -DMD_PLATFORM=linux -DMD_BUILD_TYPE=release
```

3\. Build:

```shell
make -j$(nproc)
```
4\. Built library will be here (for 64-bit Linux):

```shell
(project_root)/dump/linux64/release/md/libmd.so
```

*Note: To clear CMake params remove CMakeCache.txt, then regenerate.*

##
___(*) Other names and brands my be claimed as property of others.___
