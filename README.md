# Rocket Launch Sequence
Ludum Dare 50: Delay The Inevitable

Author: Timothy Johnson <br>
Date: April 1, 2022 to April 4, 2022

A pixel-art 2D top-down puzzle-platformer where you stall a rocket launch by completing vital safety systems.
Solve mini-games under pressure, race against the countdown, and launch when all systems are green.

## Overview

&nbsp;&nbsp;&nbsp;&nbsp;Rocket Launch Sequence is a 2D top-down puzzle-platformer developed in Unity for Ludum Dare 50, where the theme was “Delay the Inevitable.”

&nbsp;&nbsp;&nbsp;&nbsp;You play as a technician trapped in a high-stakes rocket launch scenario.
A countdown is active, but the rocket isn't ready.
Your job is to delay the inevitable launch by solving a series of systems puzzles scattered around the facility. Once all systems are secure, initiate the launch sequence.

🎯 Game Jam Theme Integration

The theme “Delay the Inevitable” is central to gameplay. The rocket will launch, but you can delay it by interacting with and solving crucial system puzzles.
The twist: you can't stop the launch—only buy time to make it safe.

🧩 Features

    🎮 Top-down pixel-art movement with real-time puzzle solving

    ⏱️ Launch timer to pressure the player

    🧠 Three unique mini-games, each representing a system check

    🧍‍♂️ Interactable objects across a tiled environment

    🔄 Dynamic task-tracking and state transitions

    🎇 Multiple endings depending on launch readiness

🎮 Gameplay
    
    Explore the command center and interact with key terminals to activate puzzles.
    Completing each mini-game delays the countdown and updates the launch system’s status.
    
    Solve all three to enable a safe launch. Fail to do so in time, and the rocket launches unsafely, triggering a failure state.

🧪 Mini-Games

    🧭 Compass Puzzle
    
    Rotate four quarter-circle tiles to form a complete compass.
    Each tile rotates 90° per click.
    🚰 Pipe Connection Puzzle
    
    Rotate and align pipe tiles to ensure water flows from input to output.
    Leaks or dead ends = system failure.
    🧩 Matching Puzzle
    
    Match scattered components from the ground onto a workstation table.
    Drag and drop based on color, shape, or icon clues.

### Controls:

| Key   | Action     |
| ----- | ---------- |
| ↑ / W | Move Up    |
| ↓ / S | Move Down  |
| ← / A | Turn Left  |
| → / D | Turn Right |
| E     | Interact   |
| ESC   | Quit       |

📁 Code Structure

. <br>
Assets/ <br>
├── Scripts/ <br>
│   ├── PlayerController.cs <br>
│   ├── PuzzleManager.cs <br>
│   ├── CompassPuzzle.cs <br>
│   ├── PipePuzzle.cs <br>
│   ├── MatchPuzzle.cs <br>
│   ├── GameTimer.cs <br>
│   └── GameStateManager.cs <br>
├── Scenes/ <br>
│   ├── MainScene.unity <br>
│   ├── CompassPuzzle.unity <br>
│   ├── PipePuzzle.unity <br>
│   └── MatchPuzzle.unity <br>
├── Prefabs/ <br>
├── Sprites/ <br>
│   ├── player.png <br>
│   ├── environment_tiles.png <br>
│   ├── UI/ <br>
│   └── puzzles/ <br>

⚙️ How It Works

    The launch timer begins when the game starts.

    Each system puzzle is tied to an interactable console.

    While solving a puzzle, the global timer pauses.

    Once a puzzle is completed, the associated system is marked "Ready".

    After all systems are green, the player can launch the rocket.

    If time expires before all systems are solved, the rocket crashes after launching.
    
🖼️ Screenshots / Visuals

![ldbanner](https://github.com/user-attachments/assets/ec40cbc7-2bf2-49f8-8dcc-01802bc08935)

🧰 Technologies Used

    🎮 Unity 2021

    💻 C# scripting

    🎨 Pixel-art sprites and tilesets

    🎬 Unity Timeline (for cutscenes/animation)

    🧠 Custom FSM (Finite State Machine) for game flow

🚀 Getting Started

    To run the game locally:

    1. Clone the repository

        git clone https://github.com/MrTimmyJ/rocket-launch-sequence-unity.git
        cd rocket-launch-sequence-unity


    2. Open with Unity Hub

       Open the folder in Unity (Unity 2021 or newer recommended)

    3. Play the Game
    
       Open MainScene.unity and press ▶️ in the Unity Editor.

🌱 Planned Features

    🧭 Minimap showing player and AI progress

    🏎️ Drift mechanics or acceleration system

    🛠️ Editor for visually setting up AI.txt points

    🧊 Obstacles and power-down tiles

    🧍 2-player local multiplayer

    🧪 Better collision detection and track limits

🪪 License

This open-source project is available under the [MIT License](https://opensource.org/license/mit).

