cmake_minimum_required(VERSION 3.11)
project(MD5Encrypter)

set(CMAKE_MODULE_PATH ${CMAKE_BINARY_DIR} ${CMAKE_MODULE_PATH})


SET(CMAKE_CXX_STANDARD 11)
SET(CMAKE_CXX_STANDARD_REQUIRED ON)

find_package(Poco REQUIRED)

add_executable(md5 md5.cpp)
target_link_libraries(md5 Poco::Poco)
