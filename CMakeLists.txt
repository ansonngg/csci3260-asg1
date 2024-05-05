cmake_minimum_required(VERSION 3.28)
project(Csci3260Asg1)

set(CMAKE_CXX_STANDARD 14)

find_package(glfw3 REQUIRED)
find_package(GLEW REQUIRED)
find_package(glm REQUIRED)

set(CMAKE_RUNTIME_OUTPUT_DIRECTORY ${CMAKE_SOURCE_DIR})

add_executable(${CMAKE_PROJECT_NAME} main.cpp)

target_link_libraries(${CMAKE_PROJECT_NAME} PRIVATE glfw GLEW::GLEW glm::glm-header-only)
