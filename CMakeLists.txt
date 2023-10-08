cmake_minimum_required(VERSION 3.10)
project(MeinKraft)

set(CMAKE_CXX_STANDARD 17)
set(CMAKE_CXX_STANDARD_REQUIRED ON)

find_package(OpenGL REQUIRED)
find_package(glfw3 REQUIRED)
find_package(OpenAL REQUIRED)

add_executable(MeinKraft main.cpp)

target_link_libraries(MeinKraft OpenGL::GL glfw OpenAL::OpenAL)
