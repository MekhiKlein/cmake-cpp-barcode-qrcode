# Building C/C++ Barcode Reader with CMake

[![release](https://img.shields.io/github/release/Dynamsoft/cmake.svg)](https://github.com/Dynamsoft/cmake/releases/latest)
[![Travis CI status](https://img.shields.io/travis/dynamsoft/cmake/master?label=Travis%20CI&logo=travis)](https://travis-ci.com/github/Dynamsoft/cmake)

## What You Should Know
- [![](https://img.shields.io/badge/Download-Offline%20SDK-orange)](https://www.dynamsoft.com/barcode-reader/downloads) 
- [![](https://img.shields.io/badge/Get-30--day%20FREE%20Trial%20License-blue)](https://www.dynamsoft.com/customer/license/trialLicense/?product=dbr)

## Supported Platforms
- Windows x86/x64
- Linux x64/ARM64
- macOS x64 
- Raspberry Pi ARMv7

## Setting License
Set the license key in `BarcodeReader.cxx`:

```cpp
reader.InitLicense("LICENSE-KEY");
```

## Contact Us
- support@dynamsoft.com
- https://www.dynamsoft.com/Company/Contact.aspx

## Windows
1. Create a **build** folder:
    ```
    mkdir build
    cd build
    ```
2. Configure and build the project:
    ```bash
    // x86
    cmake -DCMAKE_GENERATOR_PLATFORM=x86 ..

    // x64
    cmake -DCMAKE_GENERATOR_PLATFORM=x64 ..
    
    cmake --build . --config release
    ```
3. Run the app:
    ```
    Release\BarcodeReader [image-file] [optional: license-file] [optional: template-file]
    ```

## Linux and Raspberry Pi OS
1. Install **CMake**:
    ```bash
    sudo apt-get install cmake
    ```
2. Create a **build** folder:
    ```
    mkdir build
    cd build
    ```
3. Configure and build the project:
    ```bash
    cmake ..
    # cmake -DARM32_BUILD=TRUE ..
    cmake --build . --config release 
    ```
4. Run the app:
    ```
    ./BarcodeReader [image-file] [optional: license-file] [optional: template-file]
    ```

## macOS 
1. Install **CMake**:
    ```bash
    brew install cmake
    ```
2. Create a **build** folder:

    ```
    mkdir build
    cd build
    ```

3. Configure and build the project:

    ```bash
    cmake ..
    cmake --build . --config release 
    ```

4. Run the app:

    ```
    ./BarcodeReader [image-file] [optional: license-file] [optional: template-file]
    ```

## Screenshot

![Raspberry Pi Barcode Reader](https://www.codepool.biz/wp-content/uploads/2016/03/rpi_dbr_result.png)

## Reference
* https://cmake.org/cmake-tutorial/
* https://cmake.org/Wiki/CMake_Useful_Variables
* https://stackoverflow.com/questions/10671916/how-to-copy-dll-files-into-the-same-folder-as-the-executable-using-cmake
* https://cmake.org/Wiki/CMake_RPATH_handling

## Blog
* [CMake: Build C++ Project for Windows, Linux and macOS](http://www.codepool.biz/cmake-cc-windows-linux-macos.html)
* [My First C/C++ App Built with CMake on Windows](http://www.codepool.biz/cc-barcode-app-cmake-windows.html)
