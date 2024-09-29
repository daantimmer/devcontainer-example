
if (CMAKE_SYSTEM_NAME STREQUAL "Generic-ELF") # see: cmake/toolchain-arm-gcc.cmake

  add_executable(example_target.embedded)

  target_sources(example_target.embedded PRIVATE
    main.cpp
  )

  target_link_libraries(example_target.embedded PRIVATE
    example_app
  )

endif()
