cmake_minimum_required(VERSION 3.13)
set(CMAKE_CXX_STANDARD 17)
project(GLFW-Test)

add_executable(glfw-test main.cpp)

add_subdirectory(third-party/glfw)
target_include_directories(glfw-test third-party/glfw/include)
target_link_libraries(glfw-test glfw ${GLFW_LIBRARIES})
