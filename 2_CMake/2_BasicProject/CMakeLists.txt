# 0.) Create code and CMake File
# 1.) mkdir build
# 2.) cd build
# 3.) cmake ..
# 4.) cmake --build . --target Library
# 5.) cmake --build . --target Executable
# 6.) ./Executable
cmake_minimum_required(VERSION 3.16)

project(CppProjectTemplate VERSION 1.0.0 LANGUAGES C CXX)

add_library(Library STATIC my_lib.cc)

add_executable(Executable main.cc)

target_link_libraries(Executable PUBLIC Library)
