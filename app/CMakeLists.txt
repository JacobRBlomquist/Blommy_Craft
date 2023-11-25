add_executable(BlommyApp main.cpp)

target_link_libraries(BlommyApp PRIVATE glfw)
target_link_libraries(BlommyApp PRIVATE OpenGL::GL)