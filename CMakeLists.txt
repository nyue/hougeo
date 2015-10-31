cmake_minimum_required(VERSION 2.8)
project( "hougeo" )

IF ( NOT WIN32 )
  ADD_DEFINITIONS ( -fPIC )
ENDIF ()

IF (APPLE)
  ADD_DEFINITIONS ( -std=c++11 )
ENDIF ()

# hougeo library ---
add_subdirectory( hougeo )

# test and demo applications ---
add_subdirectory( tests )
