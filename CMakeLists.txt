cmake_minimum_required(VERSION 3.16.3)

project(orange)

add_executable(${PROJECT_NAME} main.cpp)

add_subdirectory(peeler)
target_link_libraries(${PROJECT_NAME} PRIVATE peeler)
target_include_directories(${PROJECT_NAME} PRIVATE peeler/)
