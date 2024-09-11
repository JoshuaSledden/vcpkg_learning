cmake_minimum_required(VERSION 3.29)
project(vcpkg_learning)

set(CMAKE_CXX_STANDARD 20)

add_executable(vcpkg_learning main.cpp)

find_package(nlohmann_json CONFIG REQUIRED)
target_link_libraries(vcpkg_learning PRIVATE nlohmann_json::nlohmann_json)