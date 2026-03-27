add_library(dearmarkdown STATIC 
	markdown.cpp
	md4c.c
)

target_include_directories(dearmarkdown PUBLIC "${CMAKE_CURRENT_SOURCE_DIR}")