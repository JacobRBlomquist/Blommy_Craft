cmake_minimum_required(VERSION 3.15...3.27)

set(CMAKE_TOOLCHAIN_FILE ${CMAKE_CURRENT_SOURCE_DIR}/vcpkg/scripts/buildsystems/vcpkg.cmake CACHE STRING "VCPKG Toolchain File")

project(
    Blommy
    VERSION 0.1
    LANGUAGES CXX
    )

find_package(glfw3 CONFIG REQUIRED)
find_package(glad CONFIG REQUIRED)
find_package(OpenGL REQUIRED)

add_subdirectory(app)