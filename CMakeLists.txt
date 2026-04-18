cmake_minimum_required(VERSION 3.29.0)
project(planning
    VERSION 0.0.1
    DESCRIPTION "A demo of cmake planning"
    HOMEPAGE_URL "https://github.com/lychee75869/camke_plannnig_demi"
    LANGUAGES CXX
)
#设置C++标准 C++17
SET(CMAKE_CXX_STANDARD 17)
SET(CMAKE_CXX_STANDARD_REQUIRED ON)

#变量设置
set(Process ${CMAKE_SOURCE_DIR}/src/process)#process路径
set(Pnc_Map ${CMAKE_SOURCE_DIR}/src/pnc_map)#pnc_map路径
set(CMAKE_RUNTIME_OUTPUT_DIRECTORY ${PROJECT_SOURCE_DIR}/bin)
set(CMAKE_LIBRARY_OUTPUT_DIRECTORY ${PROJECT_SOURCE_DIR}/lib)

#添加子目录
add_subdirectory(src)

