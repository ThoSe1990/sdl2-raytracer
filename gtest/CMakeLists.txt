set(target unittests)

find_package(GTest)

if(GTest_FOUND)

  add_executable(${target} 
    ${CMAKE_CURRENT_SOURCE_DIR}/test.cc
  )
  target_link_libraries(${target} GTest::gtest_main)

endif()