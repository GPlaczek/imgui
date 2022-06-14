file(GLOB imgui_src CONFIGURE_DEPENDS "*.h" "*.cpp" "backends/imgui_impl_glfw.*" "backends/imgui_impl_opengl3*")
add_library(imgui ${imgui_src})

target_include_directories(imgui PUBLIC .)
target_link_directories(imgui PUBLIC .)
