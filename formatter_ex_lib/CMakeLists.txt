cmake_minimum_required(VERSION 3.4)
project(laba_ex3)
add_library(formatter_ex STATIC 
	formatter_ex.cpp
	formatter_ex.h)
set_target_properties(formatter_ex PROPERTIES
	CXX_STANDART 11
	CXX_STANDART_REQUIRED ON)
target_include_directories(formatter_ex PUBLIC
	${CMAKE_CURRENT_SOURCE_DIR}/../formatter_lib)
target_link_libraries(formatter_ex formatter) 
