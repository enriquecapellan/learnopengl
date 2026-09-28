cmake_minimum_required(VERSION 4.1)
project(learnopengl)

set(CMAKE_CXX_STANDARD 20)

find_package(glfw3 3.5 REQUIRED)
find_package(OpenGL REQUIRED)

add_library(glad STATIC external/glad/src/glad.c)
target_include_directories(glad PUBLIC external/glad/include)

add_executable(learnopengl main.cpp)
target_link_libraries(learnopengl PRIVATE glad glfw OpenGL::GL)