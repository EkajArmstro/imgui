cmake_minimum_required(VERSION 3.28)

project(imgui)

set(SOURCE_FILES
	imconfig.h
	imgui.cpp
	imgui.h
	imgui_demo.cpp
	imgui_draw.cpp
	imgui_internal.h
	misc/cpp/imgui_stdlib.cpp
	misc/cpp/imgui_stdlib.h
	imgui_tables.cpp
	imgui_widgets.cpp
	imstb_rectpack.h
	imstb_textedit.h
	imstb_truetype.h
)
source_group("" FILES ${SOURCE_FILES})

add_library(imgui ${SOURCE_FILES})

target_include_directories(imgui PUBLIC .)
