WINDOWS:

Install MinGW (mingw32-base-bin and mingw32-gcc-g++-bin) and CMAKE.

Add the C:\Program Files\CMake\bin and C:\MinGW\bin to the environment variable PATH.

mkdir build
cd build
cmake .. -G "MinGW Makefiles"
mingw32-make

And to execute:
./../binary/MyApplication
./../binary/UnitTests


