if (CMAKE_SYSTEM_NAME STREQUAL "Windows")

  add_executable(example_target.windows)

  target_sources(example_target.windows PRIVATE
    main.cpp
  )

  target_link_libraries(example_target.windows PRIVATE
    example_app
  )

endif()
