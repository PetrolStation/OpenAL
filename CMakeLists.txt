cmake_minimum_required(VERSION 3.16)

PA_NEW(OpenAL)

PA_INCLUDE_DIRECTORIES(
    ${CMAKE_CURRENT_SOURCE_DIR}/src
    ${CMAKE_CURRENT_SOURCE_DIR}/deps/openal-soft/include
)

PA_LINK_LIBRARIES(OpenAL)

File(GLOB_RECURSE SOURCE_FILES src/*.cpp )
File(GLOB_RECURSE HEADER_FILES src/*.h   )

PA_ADD_SOURCE_FILES(
    ${SOURCE_FILES}
    ${HEADER_FILES}
)

add_subdirectory(deps)