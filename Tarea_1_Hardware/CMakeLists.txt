cmake_minimum_required(VERSION 3.26)
project(Barberia)

file(GLOB_RECURSE SRC CONFIGURE_DEPENDS
	"${CMAKE_CURRENT_SOURCE_DIR}/src/*.c"
	"${CMAKE_CURRENT_SOURCE_DIR}/include/*.h"
)

add_executable(${PROJECT_NAME} ${SRC})

target_include_directories(Barberia PUBLIC ${CMAKE_CURRENT_SOURCE_DIR}/include)