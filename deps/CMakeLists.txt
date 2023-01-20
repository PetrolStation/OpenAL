# openal-soft
set( ALSOFT_UTILS          OFF CACHE BOOL "Build utility programs"                     FORCE )
set( ALSOFT_NO_CONFIG_UTIL ON  CACHE BOOL "Disable building the alsoft-config utility" FORCE )

add_subdirectory(openal-soft)