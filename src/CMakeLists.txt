add_library(mazeGen mazeGen.cpp)
target_include_directories(mazeGen PUBLIC ${PROJECT_SOURCE_DIR}/include)

add_library(mazeSolve mazeSolve.cpp)
target_include_directories(mazeSolve PUBLIC ${PROJECT_SOURCE_DIR}/include)
