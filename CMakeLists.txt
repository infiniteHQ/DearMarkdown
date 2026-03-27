add_library(dearmarkdown STATIC 
	markdown.cpp
	md4c.c
)

target_link_libraries(dearmarkdown PUBLIC imgui SDL2-static)
target_include_directories(dearmarkdown PUBLIC "${CMAKE_CURRENT_SOURCE_DIR}")