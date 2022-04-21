cmake_minimum_required ( VERSION 3.0 )

FILE ( GLOB SOURCES_FILE
    *.cpp
    *.hpp
)

TARGET_SOURCES ( MemoryReader PRIVATE
    ${SOURCES_FILE}
)
