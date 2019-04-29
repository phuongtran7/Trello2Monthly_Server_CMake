# CMakeList.txt : CMake project for Trello2Monthly_Server_CMake, include source and define
# project specific logic here.
#
cmake_minimum_required (VERSION 3.8)

# Add source to this project's executable.
add_executable (Trello2Monthly_Server_CMake "Trello2Monthly_Server_CMake.cpp" "Trello2Monthly_Server_CMake.h")
find_package(cpprestsdk REQUIRED)
target_link_libraries(CMake_Trello2Monthly PRIVATE cpprestsdk::cpprest)
find_package(spdlog CONFIG REQUIRED)
target_link_libraries(CMake_Trello2Monthly PRIVATE spdlog::spdlog)

# TODO: Add tests and install targets if needed.
