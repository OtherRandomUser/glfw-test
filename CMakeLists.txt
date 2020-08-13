cmake_minimum_required(VERSION 3.13)
set(CMAKE_CXX_STANDARD 17)
project(GLFW-Test)

add_executable(glfw-test main.cpp)

find_package(OpenGL REQUIRED)

add_subdirectory(${CMAKE_CURRENT_SOURCE_DIR}/third-party/glfw)

target_include_directories(glfw-test
    PUBLIC
        third-party/glfw/include
)

target_link_libraries(glfw-test glfw OpenGL::GL)
