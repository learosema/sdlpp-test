# Learning SDL2 and SDL2pp

This is a little repo for me to learn SDL2 and SDL2pp using C++.

I'm roughly orienting on the libSDL2pp tutorial: <https://github.com/libSDL2pp/libSDL2pp-tutorial>.

## Build process

This project relies on CMake. `cmake .` creates a Makefile for you which you can use to build the project via `make`. In case you are using Visual Studio Code, the CMake extension can do this for you.

## Apps

- <b>test1</b>: open a black window. This is more or less lesson-02 in the tutorial, but without images but with the event poll. The window is closed when `[Q]` or `[ESC]` is pressed.
