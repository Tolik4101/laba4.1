cmake_minimum_required(VERSION 3.4)
project(solverapp)
add_executable(solverexe equation.cpp)
set_target_properties(solverexe PROPERTIES
	CXX_STANDART 11
	CXX_STANDART_REQUIRED ON)
target_include_directories(solverexe PUBLIC
	${CMAKE_CURRENT_SOURCE_DIR}/../formatter_ex_lib)
target_include_directories(solverexe PUBLIC
        ${CMAKE_CURRENT_SOURCE_DIR}/../solver_lib)
target_link_libraries(solverexe formatter_ex)
target_link_libraries(solverexe solver)
