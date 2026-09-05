cmake_minimum_required(VERSION 3.15)
project(surelog_consumer LANGUAGES CXX)

find_package(Surelog CONFIG REQUIRED)

add_executable(surelog_consumer main.cpp)
target_link_libraries(surelog_consumer PRIVATE surelog::surelog)
