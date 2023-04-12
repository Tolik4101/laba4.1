cmake_minimum_required(VERSION 3.4)
#Указание минимальной версии сборки
project(laba3)
#Называем проект
add_library(formatter STATIC 
	formatter.cpp
	formatter.h)
#Называем библиотеку, ее тип и указываем файлы, которые будут подключены
set_target_properties(formatter PROPERTIES
	CXX_STANDART 11
	CXX_STANDART_REQUIRED ON)
#Указываем свойства библиотеки
