PROJECT(osgcairodistancefield)

LINK_LIBRARIES(osgCairo
    ${OSGDB_LIBRARY}
    ${OSGGA_LIBRARY}
    ${OSGVIEWER_LIBRARY}
)

ADD_EXECUTABLE(osgcairodistancefield osgcairodistancefield.cpp)

INSTALL(TARGETS osgcairodistancefield DESTINATION ${CMAKE_INSTALL_PREFIX}/bin)
SET_TARGET_PROPERTIES(osgcairodistancefield PROPERTIES DEBUG_POSTFIX "${CMAKE_DEBUG_POSTFIX}")
