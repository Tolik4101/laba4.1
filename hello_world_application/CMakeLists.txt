cmake_minimum_required(VERSION 3.4)
project(laba3_work)
add_executable(hello_world hello_world.cpp) 
set_target_properties(hello_world PROPERTIES
	CXX_STANDART 11
	CXX_STANDART_REQUIRED ON)
target_include_directories(hello_world PUBLIC
	${CMAKE_CURRENT_SOURCE_DIR}/../formatter_ex_lib)
target_link_libraries(hello_world formatter_ex)
