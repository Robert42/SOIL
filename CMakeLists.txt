cmake_minimum_required(VERSION 3.1)

add_library(soil STATIC src/image_DXT.c src/image_DXT.h src/image_helper.c src/image_helper.h src/SOIL.c include/SOIL/SOIL.h src/stbi_DDS_aug.h src/stbi_DDS_aug_c.h src/stb_image_aug.c src/stb_image_aug.h)
target_include_directories(soil PUBLIC include)
target_link_libraries(soil glew)
