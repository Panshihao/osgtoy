SET( LIB_NAME osgdb_dem )

ADD_OSGPLUGIN( ${LIB_NAME}
    ReaderWriterDEM.cpp
)

INCLUDE(ModuleInstall OPTIONAL)
