cmake_minimum_required(VERSION 3.6)
project(scheduler)

set(CMAKE_CXX_STANDARD 11)
include_directories("/Users/luke/github/homebrew/Cellar/libevent/2.1.8/include")
link_directories("/Users/luke/github/homebrew/Cellar/libevent/2.1.8/lib")



set(SOURCE_FILES heap_based.cpp libevent_based.cpp)
add_executable(scheduler ${SOURCE_FILES})
target_link_libraries(scheduler event)
