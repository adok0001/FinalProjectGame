# CMakeList.txt : CMake project for FinalProject, include source and define
# project specific logic here.
#
cmake_minimum_required (VERSION 3.8)

project (FinalProject)

# Add source to this project's executable.
add_executable (FinalProject "FinalProjectGame.cpp" "FinalProject.h" "Player.h" "Tetris.h" "GameController.h")

# TODO: Add tests and install targets if needed.
target_include_directories(FinalProject PUBLIC "sfml/include")
target_link_directories(FinalProject PUBLIC "sfml/lib")
target_link_libraries(FinalProject PUBLIC "openal32.dll")
target_link_libraries(FinalProject PUBLIC "sfml-system-d.dll")
target_link_libraries(FinalProject PUBLIC "sfml-window-d.dll")
target_link_libraries(FinalProject PUBLIC "sfml-graphics-d.dll")