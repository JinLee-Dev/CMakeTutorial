cmake_minimum_required(VERSION 3.10)

#set project name
project(Tutorial2 
	LANGUAGES CXX
	VERSION 1.2.7
)

#add PrintModule library
add_subdirectory(PrintModule)

#add the executable
add_executable(Tutorial2
		main.cpp
)

#link PrintModule
target_link_libraries(Tutorial2 PUBLIC PrintModule)
