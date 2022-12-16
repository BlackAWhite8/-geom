# CMakeList.txt: файл проекта CMake верхнего уровня; проведите глобальную конфигурацию
# и включите сюда подпроекты.
#
cmake_minimum_required (VERSION 3.8)

project ("geomLib")

include_directories(.)

add_subdirectory ("geomLib")



add_executable (geomLib.test
geomLib.test.cpp

)

target_link_libraries(geomLib.test geomLib)