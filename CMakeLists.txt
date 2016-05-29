cmake_minimum_required(VERSION 2.8)
project(simple-hash-library)

set(CMAKE_CXX_FLAGS "${CMAKE_CXX_FLAGS} -D_GLIBCXX_USE_CXX11_ABI=0 -std=c++11")

file(GLOB SHL_SOURCE_FILES
  "*.cpp"  
)

add_library(shl STATIC
            ${SHL_SOURCE_FILES})
