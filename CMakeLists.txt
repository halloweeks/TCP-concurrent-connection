cmake_minimum_required(VERSION 3.10)

set(CMAKE_CXX_STANDARD 17)
set(CMAKE_CXX_STANDARD_REQUIRED ON)

project(networking VERSION 1.0)

include_directories(include)

add_executable(server.exe server.cpp)
add_executable(client.exe client.cpp)

target_link_libraries(server.exe pthread)