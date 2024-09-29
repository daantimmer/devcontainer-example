if (CMAKE_SYSTEM_NAME STREQUAL "Darwin")

  add_executable(example_target.darwin)

  target_sources(example_target.darwin PRIVATE
    main.cpp
  )

  target_link_libraries(example_target.darwin PRIVATE
    example_app
  )

endif()
