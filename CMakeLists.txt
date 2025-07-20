cmake_minimum_required(VERSION 3.23)

#project(thread_pool LANGUAGES CXX)
set(CMAKE_CXX_STANDARD 17)
set(CMAKE_CXX_STANDARD_REQUIRED ON)

add_library(thread_pool INTERFACE)

install(TARGETS thread_pool
		EXPORT libTargets
		LIBRARY DESTINATION lib
		ARCHIVE DESTINATION lib
		RUNTIME DESTINATION bin
		INCLUDES DESTINATION include)

install(DIRECTORY include/ DESTINATION include)

set(LIB_TARGETS thread_pool PARENT_SCOPE)