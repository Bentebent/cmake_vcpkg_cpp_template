find_package(GTest CONFIG REQUIRED)
include(GoogleTest)

set(TEST_SOURCE_FILES
		demo_test.cpp
		main.cpp
		)

add_executable(placeholder_tests ${TEST_SOURCE_FILES})
target_link_libraries(placeholder_tests PRIVATE GTest::gtest)

gtest_discover_tests(placeholder_tests)