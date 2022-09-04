cmake_minimum_required(VERSION 3.9)

project(test6)

# set(CMAKE_CXX_STANDARD 11)
# SET(CMAKE_BUILD_TYPE Debug)
# set(CMAKE_C_FLAGS_DEBUG "$ENV{CXXFLAGS} -O0 -Wall -g")
# set(CMAKE_CXX_FLAGS_DEBUG "$ENV{CXXFLAGS} -O0 -Wall -g")
include_directories(.)
include_directories(/usr/local/include)
include_directories(glm)
link_directories(/usr/local/lib)

add_executable(test6 test6_3Dcoord.cpp glad.c shader_s.h stb_image.h)
target_link_libraries(test6 glfw)