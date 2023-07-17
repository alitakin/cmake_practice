# cmake_practice
This repository serves as a sandbox for experimenting with CMake. It functions as a playground where ideas are explored without serious implications.


How to build and Run
==============
(only tested on Ubuntu 22.04 LTS)
First Navigate to the root directory e.g same directory with the top/first CMakeLists.txt

then

        mkdir build
        cd build
then 


        cmake ..

then 


        make -j8
        (or make -j$(nproc))

To run 


    ./cmake_practice_app




