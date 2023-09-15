cmake_minimum_required(VERSION 3.1.0)

project(hello VERSION 1.0.0 LANGUAGES CXX)


set(CMAKE_CXX_STANDARD 11)
set(CMAKE_CXX_STANDARD_REQUIRED ON)

set(CMAKE_AUTOMOC ON)
set(CMAKE_AUTORCC ON)
set(CMAKE_AUTOUIC ON)

find_package(Qt5 COMPONENTS Widgets REQUIRED)

add_executable(hello
    main.cpp
)

target_link_libraries(hello Qt5::Widgets)
