include(../cmake/GtsamTesting.cmake)
include(../cmake/GtsamBuildTypes.cmake)

set (excluded_examples
    "elaboratePoint2KalmanFilter.cpp"
    "Pose3SLAMExample_g2o.cpp"   # addon y.w.
    "Pose2SLAMExample_g2o.cpp"   # addon y.w.
)

include_directories(${CMAKE_SOURCE_DIR}) # addon y.w.

gtsamAddExamplesGlob("*.cpp" "${excluded_examples}" "gtsam::gtsam;gtsam_unstable;${Boost_PROGRAM_OPTIONS_LIBRARY}")
