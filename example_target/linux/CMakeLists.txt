if (CMAKE_SYSTEM_NAME STREQUAL "Linux")

  add_executable(example_target.linux)

  target_sources(example_target.linux PRIVATE
    main.cpp
  )

  target_link_libraries(example_target.linux PRIVATE
    example_app
  )

endif()
