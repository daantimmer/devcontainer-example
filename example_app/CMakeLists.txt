add_library(example_app STATIC)

target_sources(example_app
    PRIVATE
        application.cpp
        application.hpp
)

target_include_directories(example_app
    PUBLIC
        ${CMAKE_CURRENT_SOURCE_DIR}/../
)

target_link_libraries(example_app
    PUBLIC
        example_lib
)
