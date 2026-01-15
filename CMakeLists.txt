cmake_minimum_required(VERSION 3.13)
project(my_python_ros2_pkg)

find_package(ament_cmake REQUIRED)
find_package(ament_cmake_python REQUIRED)

# Install Python modules
ament_python_install_package(
  ${PROJECT_NAME}
  PACKAGE_DIR
    src/${PROJECT_NAME}
  VERSION
    ${PROJECT_VERSION}
  SCRIPTS_DESTINATION
    lib/${PROJECT_NAME}
) 

ament_package()
