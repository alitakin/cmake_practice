cmake_minimum_required(VERSION 3.10)
project(cmake_practice)

add_subdirectory(internal/lib_1)
add_subdirectory(internal/lib_2)
add_subdirectory(internal/lib_3)

add_executable(cmake_practice_app main.cpp)

target_link_libraries(cmake_practice_app Lib_1 Lib_2 Lib_3)

#target_link_libraries(MyApp Lib1 Lib2 Lib3)

target_include_directories(cmake_practice_app PUBLIC
    ${CMAKE_CURRENT_SOURCE_DIR}/internal/lib_1
    ${CMAKE_CURRENT_SOURCE_DIR}/internal/lib_2
    ${CMAKE_CURRENT_SOURCE_DIR}/internal/lib_3
)