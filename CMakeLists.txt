cmake_minimum_required(VERSION 3.1.0)

find_package(Qt5Core REQUIRED)
find_package(Qt5GUI REQUIRED)
set(CMAKE_AUTOMOC ON)

add_executable(main main.cpp openglwindow.cpp)
target_include_directories(main PUBLIC .)
target_link_libraries(main Qt5::Core)
target_link_libraries(main Qt5::Gui)
