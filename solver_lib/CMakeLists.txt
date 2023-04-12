cmake_minimum_required(VERSION 3.4)
project(solverlab)
add_library(solver STATIC 
	solver.cpp
	solver.h)
set_target_properties(solver PROPERTIES
	CXX_STANDART 11
	CXX_STANDART_REQUIRED ON)
	
