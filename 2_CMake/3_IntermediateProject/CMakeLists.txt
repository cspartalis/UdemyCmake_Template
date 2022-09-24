cmake_minimum_required(VERSION 3.16)

project(CppProjectTemplate VERSION 1.0.0 LANGUAGES C CXX)

add_subdirectory(src)   # It must be defined before app
add_subdirectory(app)
