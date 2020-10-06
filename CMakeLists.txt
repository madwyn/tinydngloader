project(tinydng)

set(tinydng_SRCS
        tiny_dng_loader.h
        stb_image.h
        miniz.h
        miniz.c
)

include_directories(
        ${CMAKE_CURRENT_SOURCE_DIR}
)

add_library(tinydng ${tinydng_SRCS})

target_include_directories(tinydng INTERFACE ${CMAKE_CURRENT_SOURCE_DIR} )
