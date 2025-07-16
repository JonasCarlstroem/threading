cmake_minimum_required(VERSION 3.23)

#project(thread_pool LANGUAGES CXX)
set(CMAKE_CXX_STANDARD 17)
set(CMAKE_CXX_STANDARD_REQUIRED ON)

add_library(thread_pool INTERFACE)

set(LIB_TARGETS thread_pool PARENT_SCOPE)