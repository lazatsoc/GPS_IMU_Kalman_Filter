cmake_minimum_required(VERSION 3.23)
project(GPS_IMU_Kalman_Filter_master)

set(CMAKE_CXX_STANDARD 14)

include_directories(lib)

add_executable(GPS_IMU_Kalman_Filter_master
        src/ekf.cpp
        src/ekf.hpp
        src/fusion.cpp
        src/fusion.hpp
        src/geo_ned.cpp
        src/geo_ned.hpp
        src/main.cpp
        src/parameterReader.hpp
        src/run_fusion.cpp
        src/run_fusion.hpp
        src/utils.cpp
        src/utils.hpp)

configure_file(src/data.csv data.csv COPYONLY)