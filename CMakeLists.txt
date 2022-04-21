cmake_minimum_required( VERSION 3.0 )
project ( MemoryReader )

SET ( CMAKE_SHARED_LIBRARY_PREFIX "" )
SET ( CMAKE_STATIC_LIBRARY_PREFIX "" )

if ( WIN32 ) # Only windows library

    # SET ( LIBRARY_TYPE "SHARED" )
    SET ( LIBRARY_TYPE "STATIC" )

    add_library ( MemoryReader ${LIBRARY_TYPE} memory_reader_include.hpp )

    add_subdirectory( src )

endif()