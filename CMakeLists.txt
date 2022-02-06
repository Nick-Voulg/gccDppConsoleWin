cmake_minimum_required(VERSION 3.21)
project(gccDppConsoleWin)

set(CMAKE_CXX_STANDARD 11)

add_executable(gccDppConsoleWin
        DeviceIO/AsciiCmdUtilities.cpp
#        DeviceIO/AsciiCmdUtilities.h
        DeviceIO/DP5Protocol.cpp
#        DeviceIO/DP5Protocol.h
        DeviceIO/DP5Status.cpp
        DeviceIO/DP5Status.h
#        DeviceIO/DppConst.h
        DeviceIO/DppLibUsb.cpp
#        DeviceIO/DppLibUsb.h
        DeviceIO/DppUtilities.cpp
#        DeviceIO/DppUtilities.h
#        DeviceIO/libusb.h
        DeviceIO/ParsePacket.cpp
#        DeviceIO/ParsePacket.h
        DeviceIO/SendCommand.cpp
#        DeviceIO/SendCommand.h
        ConsoleHelper.cpp
#        ConsoleHelper.h
        gccDppConsole.cpp
        stringex.cpp
#        stringex.h
#        stringSplit.h
        )

#target_compile_options(gccDppConsoleWin PUBLIC -Wall -O0)

target_include_directories(gccDppConsoleWin PUBLIC
        DeviceIO
        .
        )
target_link_libraries(gccDppConsoleWin PUBLIC
        ${CMAKE_SOURCE_DIR}/DeviceIO/libusb.lib
        ws2_32.lib
        )

