cmake_minimum_required(VERSION 3.10)
project(Lime3DS)

# Set the C++ standard
set(CMAKE_CXX_STANDARD 11)
set(CMAKE_CXX_STANDARD_REQUIRED True)

# Add source files
file(GLOB_RECURSE SOURCES "src/*.cpp")

# Create the executable
add_executable(Lime3DS ${SOURCES})

# Specify target architecture
set(CMAKE_SYSTEM_PROCESSOR arm64)

# Include directories
include_directories(include)

# Link libraries if necessary
# target_link_libraries(Lime3DS <libraries>)
