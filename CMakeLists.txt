cmake_minimum_required(VERSION 3.22)
project(OpenGLPlayground)

set(CMAKE_CXX_STANDARD 17)

add_executable(OpenGLPlayground stb_image.h main.cpp)

find_package(OpenGL REQUIRED)
find_package(glfw3 REQUIRED)
find_package(GLEW REQUIRED)

target_link_libraries(OpenGLPlayground ${OPENGL_LIBRARIES} glfw ${GLEW_LIBRARIES})

