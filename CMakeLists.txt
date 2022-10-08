cmake_minimum_required(VERSION 3.16)
project(IntentReco_project)
 
#includes
include_directories(inc)
 
#Can manually add the sources using the set command as follows:
#set(SOURCES src/main.cpp src/abc.cpp)
 
#However, the file(GLOB...) allows for wildcard additions:
file(GLOB SOURCES "src/*.cpp")
 
add_executable(IntentRecogBin ${SOURCES})