cmake_minimum_required(VERSION 2.8)
project( "hougeo" )

IF (APPLE)
  ADD_DEFINITIONS ( -std=c++11 )
ENDIF ()

# hougeo library ---
add_subdirectory( hougeo )

# test and demo applications ---
add_subdirectory( tests )
