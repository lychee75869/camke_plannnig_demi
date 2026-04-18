#指定工程名
project(planning_main)
#添加子目录
add_subdirectory(pnc_map)
add_subdirectory(process)

#添加可执行文件
add_executable(${PROJECT_NAME} ${CMAKE_SOURCE_DIR}/planning_main.cpp)
#可执行文件的头文件依赖
target_include_directories(
    ${PROJECT_NAME} 
    PUBLIC 
    ${Process}
)
target_link_libraries(
    ${PROJECT_NAME}
    PUBLIC
    process
    )
