cmake_minimum_required(VERSION 3.24)
list(APPEND CMAKE_MODULE_PATH "${CMAKE_CURRENT_LIST_DIR}/cmake")

project(example LANGUAGES C CXX VERSION 1.0.0) # x-release-please-version

if (CMAKE_SYSTEM_NAME STREQUAL "Generic")
    enable_language(ASM)
endif()

set(CMAKE_CXX_STANDARD 17)
set(CMAKE_CXX_STANDARD_REQUIRED On)

set_directory_properties(PROPERTY USE_FOLDERS On)

add_subdirectory(example_app)
add_subdirectory(example_lib)
add_subdirectory(example_target)
