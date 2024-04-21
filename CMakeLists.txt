
# CMAKE_TOOLCHAIN_FILE must be set before "project(...)"
# otherwise it is ignored
set(CMAKE_TOOLCHAIN_FILE "${PROJECT_BINARY_DIR}/conan_toolchain.cmake")

Project(SLAM)
cmake_minimum_required(VERSION 3.16)

find_package(gflags REQUIRED)
find_package(Ceres REQUIRED)
find_package(GTSAM REQUIRED)


add_subdirectory(ceres_examples)
add_subdirectory(gtsam_examples)
