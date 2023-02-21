cmake_minimum_required(VERSION 3.15)

project(imgui)
set(CMAKE_CXX_STANDARD 17)

file(GLOB_RECURSE src_files CONFIGURE_DEPENDS "src/*.cpp")
add_library(${PROJECT_NAME} ${src_files})

target_include_directories(${PROJECT_NAME} PUBLIC ${CMAKE_SOURCE_DIR}/external/imgui/include)
