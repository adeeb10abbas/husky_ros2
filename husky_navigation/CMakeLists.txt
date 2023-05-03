cmake_minimum_required(VERSION 3.5)
project(husky_navigation)

if(CMAKE_COMPILER_IS_GNUCXX OR CMAKE_CXX_COMPILER_ID MATCHES "Clang")
  add_compile_options(-Wall -Wextra -Wpedantic)
endif()

# Find ament_cmake and required packages
find_package(ament_cmake REQUIRED)
find_package(rclcpp REQUIRED)

ament_package()

install(
  DIRECTORY config launch maps
  DESTINATION share/${PROJECT_NAME}
)