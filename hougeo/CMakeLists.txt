
cmake_minimum_required(VERSION 2.8)

set(CMAKE_DEBUG_POSTFIX "d")
add_library( hougeo json.cpp json.h types.h )

# additional include directories
include_directories( ${CMAKE_CURRENT_SOURCE_DIR} )

# installation
install ( FILES
  json.h
  types.h
  DESTINATION
  include/hougeo
  )
install ( DIRECTORY
  ttl
  DESTINATION
  include
  )

install ( TARGETS
  hougeo
  DESTINATION
  lib
  )
