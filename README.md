# libwpcp

[![Build Status: Linux](https://travis-ci.org/paroga/DELETE_ME_20160815.svg?branch=master)](https://travis-ci.org/paroga/DELETE_ME_20160815)
[![Build Status: Windows](https://ci.appveyor.com/api/projects/status/mn7fw3008we2ag53/branch/master?svg=true)](https://ci.appveyor.com/project/paroga/delete-me-20160815/branch/master)
[![Coverage Status](https://coveralls.io/repos/paroga/DELETE_ME_20160815/badge.svg?branch=master)](https://coveralls.io/r/paroga/DELETE_ME_20160815?branch=master)
[![MIT licensed](https://img.shields.io/badge/license-MIT-blue.svg)](https://raw.githubusercontent.com/paroga/DELETE_ME_20160815/master/LICENSE)

## Introduction

libwpcp is a lightweight library to allow any existing application to exchange data via the [(Reverse)WebProcessControlProtocol (RWPCP/WPCP)](http://wpcp.net). It comes with an optional implementation for [libwebsockets](https://libwebsockets.org) to minimize the coding effort.

## Building libwpcp

You need to install [CMake](https://cmake.org) and working C compiler. Then run `cmake /path/to/source/directoy` to generate build files, which can be compiled with `cmake --build /path/to/build/directory`.

The implementation for libwebsockets need an installation of that library on your machine. If yo do not have one, it's possible to pass `-DWPCP_BUILD_LIBWEBSOCKETS=ON` to the first `cmake` call, which will build it for you.

For building the test [check](https://libcheck.github.io/check/) must be installed. Alternatively you can pass `-DWPCP_BUILD_CHECK=ON` to the first `cmake` call to let it build for you.

## License

libwpcp is distributed under the OSI-approved MIT License. See [LICENSE](LICENSE) for details.
