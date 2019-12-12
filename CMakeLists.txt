cmake_minimum_required(VERSION 3.15)
project(OpenGL_Text)

set(CMAKE_CXX_STANDARD 14)

set(SRC_LIST main.cpp glad.c Shader.h stb_image.h stb_image.cpp camera.h DanmuPoll.cpp DanmuPoll.h)

#link directories glfw3.lib freetyped.lib
link_directories(D:/Library/Libs)
link_libraries(D:/Library/Libs/glfw3.lib)
link_libraries(freetyped.lib)

#include direcotries GLAD,GLFW,glm,Freetype
include_directories(/Library/glad/include)
include_directories(/Library/glfw-3.3/include/GLFW)
include_directories(/Library/glm-0.9.9.6/glm/glm)
include_directories(Library/ft/freetype-2.9/include)

add_executable(OpenGL_Text ${SRC_LIST})
