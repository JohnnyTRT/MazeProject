add_library(imgui_backend imgui/imgui_impl_sdlrenderer3.cpp imgui/imgui_impl_sdl3.cpp)
target_include_directories(imgui_backend PUBLIC ${PROJECT_SOURCE_DIR}/include/imgui)
target_link_libraries(imgui_backend PUBLIC imgui::imgui SDL3::SDL3)

add_library(mazeGen mazeGen.cpp)
target_include_directories(mazeGen PUBLIC ${PROJECT_SOURCE_DIR}/include)

add_library(mazeSolve mazeSolve.cpp)
target_include_directories(mazeSolve PUBLIC ${PROJECT_SOURCE_DIR}/include)



