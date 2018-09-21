set(gps_SRCS
   GpsService.cpp
)
link_libraries(pthread)
add_executable (gpsService ${gps_SRCS})
target_link_libraries (gpsService zmq protobuf boost_system boost_thread gps asn proto messages utility)

