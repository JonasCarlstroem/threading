cmake_minimum_required(VERSION 3.23)

#project(thread_pool LANGUAGES CXX)
set(CMAKE_CXX_STANDARD 17)
set(CMAKE_CXX_STANDARD_REQUIRED ON)

#add_library(thread_pool INTERFACE)
CREATE_LIB(thread_pool INTERFACE)

target_include_directories(thread_pool INTERFACE
	$<BUILD_INTERFACE:${CMAKE_CURRENT_SOURCE_DIR}/include>
	$<INSTALL_INTERFACE:include/threading>
)

INSTALL_LIB(thread_pool True threading)