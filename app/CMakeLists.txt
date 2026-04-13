find_package(SDL3 REQUIRED)
add_executable(${PROJECT_NAME} main.cpp)

target_include_directories(${PROJECT_NAME} PRIVATE ${CMAKE_SOURCE_DIR}/include)
target_link_libraries(${PROJECT_NAME} SDL3::SDL3)

