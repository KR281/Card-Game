Card Game

A C++ card game project built using SDL3.

Setup

This project uses CMake for its build configuation. The project can be build using the included CMakeLists.txt.

Asset Paths

Before running the program, please check the asset paths in:
Rendering.cpp -> Rendering::loadAssets()

The project currently expects the required assets to be located at specific paths:
void Rendering::loadAssets(){
  background = IMG_LoadTexture(renderer,"../../Assets/smiley.png"); 
  cardBack = IMG_LoadTexture(renderer,"../../Assets/cardBack.png"); 
  atlases[0] = IMG_LoadTexture(renderer,"../../Assets/Atlas0.png"); 
  atlases[1] = IMG_LoadTexture(renderer,"../../Assets/Atlas1.png"); 
  fontSmall = TTF_OpenFont("../../Assets/fonts/LMR.ttf", 16); 
  fontMed = TTF_OpenFont("../../Assets/fonts/LMR.ttf", 24); 
  fontMenu = TTF_OpenFont("../../Assets/fonts/LMR.ttf", 36); 
  fontLarge = TTF_OpenFont("../../Assets/fonts/LMR.ttf", 72); 
}
If the Assets folder is located elsewhere, update these paths to match the location of your assets.

The smiley.png and cardBack.png files are used for the background and cardBack textures. You will have to 
use your own images for these. The program may still run without those two images but the display may not be correct.

Notes
This project is a demonstration of C++ programming, game logic, rendering and asset management using SDL3.
