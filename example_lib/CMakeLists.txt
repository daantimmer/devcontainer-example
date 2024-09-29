add_library(example_lib STATIC)

target_sources(example_lib
    PRIVATE
        library.cpp
        library.hpp
)

target_include_directories(example_lib
    PUBLIC
        ${CMAKE_CURRENT_SOURCE_DIR}/../
)
