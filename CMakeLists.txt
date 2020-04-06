PROJECT(OpenGLProject)
CMAKE_MINIMUM_REQUIRED(VERSION 2.8)

SET(OpenGLProject_SRC "src/Application.cpp" "src/glad.c")

link_directories(${CMAKE_SOURCE_DIR}/lib)

INCLUDE_DIRECTORIES("include")

ADD_EXECUTABLE(OpenGLProject ${OpenGLProject_SRC})

TARGET_LINK_LIBRARIES(OpenGLProject PUBLIC glfw3)
TARGET_LINK_LIBRARIES(OpenGLProject PUBLIC opengl32)
