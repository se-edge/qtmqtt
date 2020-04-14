# Generated from data_receive.pro.

#####################################################################
## data_receive Binary:
#####################################################################

qt_add_executable(data_receive
    SOURCES
        main.cpp
    PUBLIC_LIBRARIES
        # Remove: fsanitize=fuzzer
        Qt::Mqtt
        Qt::MqttPrivate
        Qt::Test
)
