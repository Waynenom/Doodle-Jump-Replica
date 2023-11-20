# Doodle-Jump-Replica
CMU 15112_23fall Term Project

<aside>
👾 **TOPIC: Doodle Jump Replica**

</aside>

[Pre-Meeting TP0](https://www.notion.so/Pre-Meeting-TP0-5ef954fc97344261aa429ce6f1ae6582?pvs=21)

## TP0 (Due Mon Nov.20 5:pm)

### Project Proposal Components

1. **Project Description**
    - Doodle Jump Replica
    - Mainly rewrite a simplified version of Doodle Jump
    - Random platform with different functions for users
    - Random monsters, users shoot bullets to defeat the monster
    - Best score for multiple players, stars earned, level system, customized character appearance
2. **Similar Projects**
    
    [15112 Doodle Jump](https://www.youtube.com/watch?v=yrv-Go-NhpM)
    
    [GitHub - MykleCode/Pygame-DoodleJump: The simplest doodle jump made with python3 and pygame](https://github.com/MykleCode/Pygame-DoodleJump#setup)
    
    - First one is the doodle jump created by Joanne Chui in sping20 term using CMU Tkinter
        - want to improve: the interface's animation refresh rate is too slow
    - Second one is a doodle jump on GitHub using Pygame
        - want to improve: lack of diverse game modes and user interaction, try to write it without import Pygame
    - Mine will add **dynamic background** and **story mode** for Doodle Jump to create a deeply user experience.
        - Dynamic background: light and dark mode for background, add random gems during the game so that player would upgrade their bullet once they collect the gems
        - Story mode: once player reaches a specific points, they can unlock the new character and upgrade the functions of those helpful platforms
3. **Structural Plan**
    - Main
        - main framework for the game to detect start, game over, paused and restart
    - Camera
        - rolling camera: move all the game objects vertically and have the player be static to create the illusion of movement
    - Level
        - the levels will be determined by the stars collected by users and the points they made
    - Player
        - record one player after type in a new name, able to record multiple players
    - Setting
        - switch from light mode to dark mode, change the difficulty (speed of moving)
4. **Algorithmic Plan**
    - Dynamic Rolling Platforms
        - define a platform class, update platform positions by decreasing the Y-coordinates of all platforms
        - gradually increase the game's difficulty by increasing the speed of platforms, or reducing the spacing between platforms
        - introduce special platforms like spring platforms, pass-through platforms, breakable platforms, etc. to affect the player’s jumping behavior
    - Collision Detection
        - check if the character collides with any of the platforms currently on the screen. If a collision occurs, the player can continue jumping
        - check if the bullets hit the monster. If the monster is hit, then vanish the monster
        - if the player hit the monster, the game is over
    - Physical Engine
        - realize fundamental jumping and gravity effect (still checking how to do it)
5. **Timeline Plan**
    - by the DDL of TP1 after Thanksgiving, I should created the main features for the project
    - during TP1 to TP2, I will focus on optimize the visual aesthetic
6. **Version Control Plan**
    - I use GitHub to realize the version control system.
    
    [GitHub - Waynenom/Doodle-Jump-Replica: CMU 15112_23fall Term Project](https://github.com/Waynenom/Doodle-Jump-Replica)
    
    - All the updates will be push to GitHub for checking and recording
7. **Module List**
    - no other module I need to import except for CMU Tkinter
