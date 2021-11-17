# Most bacis of Cmake
This practice is to show
- how to write a CMakeLists.txt for a C++ project
- how to run cmake to build a project
- how to "hide" the building files from our codes


## how to write a Cmake file
We write CMakeLists.txt to control compilation and linking process
- what is the basic structure of CMakelists.txt
  - cmake_minimum_required
    - how to check our cmake version
  - project
  - add_execuable
    - *this command is to generate an executable file from a source file like .cpp*ss

## how to run cmake process
1. cmake . % if CMakeLists.txt is in the current dir
2. make
3. ./output

## how to seperate building files
As we know it is boring to see those MakeFile etc. in our current root folder, what we can do is to seperate those files from our cpp.

It looks like
  root
    |
    |
    ----- CMakeLists.txt
    |
    |
    ----- main.cppp
    |
    |
    ----- build

Our purpose is to leave all these building files in the folder build.
1. we entre the buid folder
  - cd build
2. we build the project with cmake
  - cmake .. 
  - % this is to say the CMakeLists.txt is in the upper directory            
3. continue with building process
  - make
  - ./out 

