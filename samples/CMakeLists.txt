cmake_minimum_required(VERSION 2.8)

include_directories(../include)

file(GLOB sources "*.cpp")
file(GLOB headers "*.h*") 

if(UNIX) 
	add_executable(../bin/matrixexe  "${sources}" "${headers}")
else()
	add_executable(matrixexe  "${sources}" "${headers}")
endif()
