PROJECT( osgVRPN )

set( CMAKE_MODULE_PATH "${osgVRPN_SOURCE_DIR}/CMakeModules;${CMAKE_MODULE_PATH}" )
INCLUDE( MacroUtils )

set( EXECUTABLE_OUTPUT_PATH ${osgVRPN_SOURCE_DIR}/bin )
set( LIBRARY_OUTPUT_PATH ${osgVRPN_SOURCE_DIR}/lib )
LINK_DIRECTORIES( ${LIBRARY_OUTPUT_PATH} )

SET( CMAKE_DEBUG_POSTFIX "D" )

FIND_PACKAGE( OSG REQUIRED )
FIND_PACKAGE( VRPN REQUIRED )

ADD_SUBDIRECTORY( src )
ADD_SUBDIRECTORY( examples )

# vim: set sw=4 ts=8 et ic ai:
