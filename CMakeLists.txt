cmake_minimum_required(VERSION 3.15)
project(bezier curves VERSION 1.0 DESCRIPTION "implementation of bezier curves in C++")
 
add_subdirectory()
 
# Create an executable
add_executable(${PROJECT_NAME}
    src/main.cpp
    # your other files...
)
 
# Linking libraries
target_link_libraries(${PROJECT_NAME}
)
 
# Specify includes
target_include_directories(${PROJECT_NAME} PRIVATE
)
 
# Set C++ version
set_target_properties(${PROJECT_NAME} PROPERTIES
    CXX_STANDARD 17
    CXX_STANDARD_REQUIRED ON
)

