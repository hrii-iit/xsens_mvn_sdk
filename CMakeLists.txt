cmake_minimum_required(VERSION 3.0.0)

include_directories(include)

file(GLOB ${PROJECT_NAME}_SDK_CPP_PATH src/*.cpp)
add_library(${PROJECT_NAME}_SDK SHARED ${${PROJECT_NAME}_SDK_CPP_PATH})
set_target_properties(${PROJECT_NAME}_SDK PROPERTIES LINKER_LANGUAGE CXX)