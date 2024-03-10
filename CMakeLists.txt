cmake_minimum_required(VERSION 3.10)
project(KDTree CXX)

# Set C++ standard
set(CMAKE_CXX_STANDARD 14)

add_library(KDTree STATIC KDTree.cpp)

# Add the include directory to the library
# So that users of the library can #include <KDTree/KDTree.h>
target_include_directories(KDTree PUBLIC .)
