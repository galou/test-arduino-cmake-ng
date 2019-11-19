cmake_minimum_required(VERSION 3.8)

# The following line must be place before project(...).
# If it was not there when first calling cmake, remove all cmake generated file.
set(CMAKE_TOOLCHAIN_FILE arduino-cmake-ng/cmake/Arduino-Toolchain.cmake)

set(ARDUINO_SDK_PATH /opt/arduino-1.8.10)
#set(ARDUINO_CMAKE_PLATFORM_BOARDS_PATH $ENV{HOME}/Arduino/hardware/arbotix/avr/boards.txt)
#set(ARDUINO_CMAKE_PLATFORM_PROPERTIES_FILE_PATH $ENV{HOME}/Arduino/hardware/arbotix/avr/platform.txt)

project(test_arduino_cmake_ng LANGUAGES C CXX ASM)

#set(ARDUINO_CMAKE_PLATFORM_BOARDS_PATH /opt/arduino-1.8.8/hardware/arbotix/avr/boards.txt)
#read_boards_properties(${ARDUINO_CMAKE_PLATFORM_BOARDS_PATH})
#get_board_id(board_id arbotix "ArbotiX Std")
get_board_id(board_id "Arduino Yún")

#register_hardware_platform($ENV{HOME}/sketchbook/hardware/arbotix)

#set(ARDUINO_DEFAULT_BOARD "ArbotiX Std")
#set(ARDUINO_DEFAULT_PROGRAMMER avrispmkii)
#set(ARDUINO_DEFAULT_PORT "dummy") # Must be specified, ignore with AVR ISPMK II

