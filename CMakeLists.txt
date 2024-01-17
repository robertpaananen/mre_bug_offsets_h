cmake_minimum_required(VERSION 3.20.0)
find_package(Zephyr REQUIRED HINTS $ENV{ZEPHYR_BASE})

project(bug)
add_subdirectory(drivers)
target_sources(app PRIVATE src/main.cpp)
target_link_libraries(app PRIVATE sensor_drivers)