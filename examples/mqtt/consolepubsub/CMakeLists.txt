# Generated from qtmqtt_sub.pro.

cmake_minimum_required(VERSION 3.14)
project(qtmqtt_sub LANGUAGES CXX)

set(CMAKE_INCLUDE_CURRENT_DIR ON)

set(CMAKE_AUTOMOC ON)
set(CMAKE_AUTORCC ON)
set(CMAKE_AUTOUIC ON)

set(INSTALL_EXAMPLEDIR "examples/mqtt/consolepubsub")

find_package(Qt6 COMPONENTS Core)
find_package(Qt6 COMPONENTS Mqtt)

add_executable(qtmqtt_sub
    configuration.h
    main_sub.cpp
)
target_compile_definitions(qtmqtt_sub PUBLIC
    QT_DEPRECATED_WARNINGS
)

target_link_libraries(qtmqtt_sub PUBLIC
    Qt::Core
    Qt::Mqtt
)

install(TARGETS qtmqtt_sub
    RUNTIME DESTINATION "${INSTALL_EXAMPLEDIR}"
    BUNDLE DESTINATION "${INSTALL_EXAMPLEDIR}"
    LIBRARY DESTINATION "${INSTALL_EXAMPLEDIR}"
)
