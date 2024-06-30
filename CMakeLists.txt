cmake_minimum_required(VERSION 3.26 FATAL_ERROR)

set(PROJECT_NAME VoukOpenGL)

project(${PROJECT_NAME})

add_executable(${PROJECT_NAME} src/main.cpp)
add_subdirectory(external/glfw)
target_link_libraries(${PROJECT_NAME} glfw)

add_subdirectory(external/glad)
target_link_libraries(${PROJECT_NAME} glad)