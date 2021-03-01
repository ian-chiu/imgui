cmake_minimum_required(VERSION 3.15)
project(imgui)

add_library(imgui "")

target_sources(imgui
    PRIVATE 
        imgui_demo.cpp 
        imgui_draw.cpp 
        imgui_tables.cpp 
        imgui_widgets.cpp 
        imgui.cpp
)

target_include_directories(imgui
    PRIVATE ${CMAKE_CURRENT_LIST_DIR}
)
