add_definitions("-DFMT_HEADER_ONLY")
add_executable(test_ring_buffer test_ring_buffer.cpp)
target_link_libraries(test_ring_buffer my_lib lib3d)

add_executable(test_async_call test_async_call.cpp)
target_link_libraries(test_async_call my_lib lib3d)

add_executable(test_synced_buffer test_synced_buffer.cpp)
target_link_libraries(test_synced_buffer my_lib lib3d)
