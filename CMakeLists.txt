cmake_minimum_required(VERSION 2.8.12)
add_compile_options(-Wall)      # add_compile_options instead of CMAKE_CXX_FLAGS in CMake 2.8.12 or newer
add_compile_options(-O3)
project (stream)
#find_package(Boost 1.68 COMPONENTS coroutine context REQUIRED)
#find_package (Threads)
#if(Boost_FOUND)
#  add_executable(fibb fibb.cpp)
#  TARGET_LINK_LIBRARIES(fibb ${MANDATORY_LIBRARIES} boost_coroutine boost_context)
#endif()
add_executable(stream_c stream.c)
add_executable(stream2 stream2.c)
#target_link_libraries(threaded pthread)

