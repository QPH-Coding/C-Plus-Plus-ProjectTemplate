cmake_minimum_required(VERSION 3.23)

project(TinyProject)

set(CMAKE_CXX_STANDARD 20)

# change or delete opts for your boost 
set(BOOST_ROOT "/usr/local/boost_1_80_0")
include_directories(/usr/local/boost_1_80_0)
link_directories(/usr/local/boost_1_80_0/stage/lib)

include_directories(${PROJECT_SOURCE_DIR}/include)

add_subdirectory(${PROJECT_SOURCE_DIR}/src)
