# Card Game

A C++ card game project built using SDL3.

## Setup

This project uses CMake for its build configuation. The project can be build using the included CMakeLists.txt.

## Asset Paths

Before running the program, please check the asset paths in:
Rendering.cpp -> Rendering::loadAssets()

The project currently expects the required assets to be located at ../../Assets relative to the working directory.
If the Assets folder is located elsewhere, update these paths to match the location of your assets.

The smiley.png and cardBack.png images are not included in the repository. You can provide your own images for these
if desired. The program may still run without those two images but the display may not be correct.

## Notes

This project is a demonstration of C++ programming, game logic, rendering and asset management using SDL3.
