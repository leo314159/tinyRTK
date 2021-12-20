cmake_minimum_required(VERSION 3.19)
project(tinyRTK C)

set(CMAKE_C_STANDARD 90)

include_directories(.)

link_libraries(ws2_32 wsock32 winmm)

add_executable(tinyRTK
        novatel.c
        rcvraw.c
        rtkcmn.c
        main.c
        rtklib.h)
