cmake_minimum_required(VERSION 3.1.0)

project( camera_calibration_opencv )


find_package( OpenCV REQUIRED )

# Enable C++11
set(CMAKE_CXX_STANDARD 11)
set(CMAKE_CXX_STANDARD_REQUIRED TRUE)


include_directories( ${OpenCV_INCLUDE_DIRS} )
add_executable( camera_calibration_opencv camera_calibration.cpp )
target_link_libraries( camera_calibration_opencv ${OpenCV_LIBS} )