cmake_minimum_required(VERSION 3.20)

project(GraphRS)

set(JSON_BuildTests OFF CACHE INTERNAL "")
add_subdirectory(third-party/json)

add_executable(main src/Main.cpp)
target_link_libraries(main PRIVATE nlohmann_json::nlohmann_json)