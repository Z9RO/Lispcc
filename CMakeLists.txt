cmake_minimum_required(VERSION 3.10)

# set the project name
project(Lispcc VERSION 0.0.1)

# specify the C++ standard
set(CMAKE_CXX_STANDARD 17)
set(CMAKE_CXX_STANDARD_REQUIRED True)

configure_file(LispccConfig.h.in LispccConfig.h)


# add the executable
add_executable(Lispcc Lispcc.cc)

target_include_directories(Lispcc PUBLIC "${PROJECT_BINARY_DIR}")