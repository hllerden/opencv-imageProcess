cmake_minimum_required(VERSION 3.16)

project(ImageProcessExercise LANGUAGES CXX)

set(CMAKE_CXX_STANDARD 17)
set(CMAKE_CXX_STANDARD_REQUIRED ON)

# find_package(QT NAMES Qt6 Qt5 REQUIRED COMPONENTS Core)
# find_package(Qt${QT_VERSION_MAJOR} REQUIRED COMPONENTS Core)
find_package(OpenCV REQUIRED )
include_directories( ${OpenCV_INCLUDE_DIRS})

add_subdirectory(main)
add_subdirectory(opencv-motionDetect)
add_subdirectory(opencv-yolo)

