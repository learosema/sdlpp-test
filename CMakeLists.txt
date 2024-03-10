cmake_minimum_required(VERSION 3.28 FATAL_ERROR)
project(SDLpptest LANGUAGES CXX)

# set up SDL2pp library
set(SDL2PP_WITH_IMAGE OFF) # if you need SDL_image support
set(SDL2PP_WITH_MIXER OFF) # if you need SDL_mixer support
set(SDL2PP_WITH_TTF OFF) # if you need SDL_ttf support
add_subdirectory(libSDL2pp)


# add compilation flags
set(CMAKE_CXX_STANDARD 20)
# add_definitions(-DDATA_PATH="${PROJECT_SOURCE_DIR}/data")

# define targets
add_executable(test1 test1.cc)
target_link_libraries(test1 PRIVATE SDL2pp::SDL2pp)
