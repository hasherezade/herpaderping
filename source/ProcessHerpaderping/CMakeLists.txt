cmake_minimum_required (VERSION 2.8)
project ( herpaderp )

set(CMAKE_CXX_FLAGS_RELEASE "${CMAKE_CXX_FLAGS_RELEASE} /MT /std:c++latest")

set (rsrc
	res/version.h
	res/resource.h
	res/resource.rc
)

set (srcs
	res/resource.h
	res/version.h
	herpaderp.cpp
	utils.cpp
)

set (hdrs
	herpaderp.hpp
	pch.hpp
	utils.hpp
)

add_executable ( ${PROJECT_NAME} ${hdrs} ${srcs} ${rsrc} main.cpp )

