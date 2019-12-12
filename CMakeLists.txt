cmake_minimum_required(VERSION 3.15)
project(OpenGL_Text)

set(CMAKE_CXX_STANDARD 14)

set(SRC_LIST main.cpp glad.c Shader.h stb_image.h stb_image.cpp camera.h DanmuPoll.cpp DanmuPoll.h)

link_directories(D:/Library/Libs)
link_libraries(D:/Library/Libs/glfw3.lib)
link_libraries(freetyped.lib)

include_directories(D:/Library/glad/include)
include_directories(D:/Library/glfw-3.3/include/GLFW)
include_directories(D:/Library/glm-0.9.9.6/glm/glm)
include_directories(D:Library/ft/freetype-2.9/include)

add_executable(OpenGL_Text ${SRC_LIST})