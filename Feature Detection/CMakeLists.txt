cmake_minimum_required(VERSION 2.8)
project( detectFeatures )
find_package( OpenCV REQUIRED )
add_executable( detectFeatures detectFeatures.cpp )
target_link_libraries( detectFeatures ${OpenCV_LIBS} )
target_link_libraries(detectFeatures ${catkin_LIBRARIES} ${OpenCV_LIBRARIES} opencv_nonfree  )
