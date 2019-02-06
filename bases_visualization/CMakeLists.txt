cmake_minimum_required (VERSION 3.5.1)
project (bases_visulatization)
find_package (PCL 1.7 REQUIRED)
set (CMAKE_CXX_STANDARD 14)

include_directories(${PCL_INCLUDE_DIRS})
link_directories(${PCL_LIBRARY_DIRS})
add_definitions(${PCL_DEFINITIONS})

add_executable(find_point find_point.cpp)

target_link_libraries(find_point ${PCL_LIBRARIES})