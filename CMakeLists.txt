cmake_minimum_required(VERSION 3.10)

# Project name
project(zed_segment_CUDA)

# Set C++ standard
set(CMAKE_CXX_STANDARD 14)
set(CMAKE_CXX_STANDARD_REQUIRED ON)

# Find the ZED SDK package
find_package(ZED 3 REQUIRED)
find_package(OpenCV REQUIRED)

# Include directories
include_directories(${ZED_INCLUDE_DIRS} ${OpenCV_INCLUDE_DIRS} /usr/local/cuda/include)

# Add the executable
add_executable(zed_segment_CUDA src/main.cpp)

# Link libraries
target_link_libraries(zed_segment_CUDA ${ZED_LIBRARIES} ${OpenCV_LIBS} cuda)