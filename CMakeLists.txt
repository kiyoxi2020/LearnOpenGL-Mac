cmake_minimum_required(VERSION 3.9)

project(test4)
# set(SRCLIST test1.cpp)

# set(CMAKE_CXX_STANDARD 11)
# SET(CMAKE_BUILD_TYPE Debug)
# set(CMAKE_C_FLAGS_DEBUG "$ENV{CXXFLAGS} -O0 -Wall -g")
# set(CMAKE_CXX_FLAGS_DEBUG "$ENV{CXXFLAGS} -O0 -Wall -g")
include_directories(.)
include_directories(/usr/local/include)
link_directories(/usr/local/lib)

add_executable(test4 test4_textures.cpp glad.c shader_s.h stb_image.h)
target_link_libraries(test4 glfw)