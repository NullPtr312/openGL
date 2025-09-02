cmake_minimum_required(VERSION 3.10)
project("main")

include_directories("./include")
link_directories("./lib")

add_executable(game ${CMAKE_SOURCE_DIR}/src/main.cpp)

target_link_libraries(game glfw3dll opengl32 glew32)
