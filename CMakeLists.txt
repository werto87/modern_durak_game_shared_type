cmake_minimum_required(VERSION 3.15)
project(library_name CXX)




add_library(library_name src/hello.cpp)
target_include_directories(library_name PUBLIC include)



set_target_properties(library_name PROPERTIES PUBLIC_HEADER "include/hello.h")
install(TARGETS library_name)
