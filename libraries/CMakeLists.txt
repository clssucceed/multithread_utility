aux_source_directory(. DIR_SRCS)
FILE (GLOB DIR_INC "./include/*.h")
add_library(my_lib STATIC ${DIR_SRCS} ${DIR_INC})
target_include_directories(my_lib PUBLIC include)

if (UNIX)
target_link_libraries(my_lib pthread)
endif(UNIX)
