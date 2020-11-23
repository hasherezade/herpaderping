cmake_minimum_required ( VERSION 2.8 )

project ( herpaderping )

include_directories ( ${PROJECT_SOURCE_DIR}/ext/submodules/wil/include )
include_directories ( ${PROJECT_SOURCE_DIR}/ext/submodules/phnt )

add_subdirectory ( source\\ProcessHerpaderping )
add_subdirectory ( ext\\submodules\\wil )
