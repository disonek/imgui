add_library(imgui STATIC)
target_sources(
  imgui
  PUBLIC    imgui_widgets.cpp
            imgui_demo.cpp
  INTERFACE imconfig.h
            imgui.h
            imgui.cpp
            imgui_draw.cpp
            imgui_internal.h
            imstb_rectpack.h
            imstb_textedit.h
            imstb_truetype.h)

target_include_directories(imgui INTERFACE  examples .)