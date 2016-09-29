cmake_minimum_required(VERSION 3.3)

project(boost_tuple)

add_library(boost_tuple INTERFACE)

target_include_directories(boost_tuple BEFORE INTERFACE ${CMAKE_CURRENT_SOURCE_DIR}/include)

install(TARGETS boost_tuple DESTINATION lib)
install(DIRECTORY ${CMAKE_CURRENT_SOURCE_DIR}/include/boost DESTINATION include)
