

  add_executable(Pose2SLAMExample_g2o Pose2SLAMExample_g2o.cpp)
  target_link_libraries(Pose2SLAMExample_g2o gtsam::gtsam)



  add_executable(Pose3SLAMExample_g2o Pose3SLAMExample_g2o.cpp)
  target_link_libraries(Pose3SLAMExample_g2o gtsam::gtsam)
