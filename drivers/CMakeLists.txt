add_library(sensor_drivers sensor_driver.cpp)
target_link_libraries(sensor_drivers PRIVATE zephyr_interface)