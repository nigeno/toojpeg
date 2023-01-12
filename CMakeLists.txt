cmake_minimum_required(VERSION 3.5)

project(jpeg_app)

file(GLOB_RECURSE LocalProjectIncludes "*.h")

set(SOURCES main.cpp
            toojpeg.cpp            
            ${LocalProjectIncludes})

add_executable(${PROJECT_NAME} ${SOURCES})
#target_include_directories(${PROJECT_NAME} PUBLIC include)