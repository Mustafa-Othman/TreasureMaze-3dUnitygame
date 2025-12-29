The Dark Maze 🧩
The Dark Maze is a first-person 3D exploration and puzzle game developed in Unity. It challenges players to navigate a complex labyrinth where environmental atmosphere and lighting are the primary mechanics.

🎮 Gameplay Overview
In The Dark Maze, the player is trapped in a mysterious labyrinth and must locate the exit to survive. The game features a progressive difficulty curve across two main stages:

Level 1 (Introductory): A brightly lit environment designed to familiarize the player with movement mechanics and maze navigation.

Level 2 (Dark Mode): A high-tension challenge where visibility is near-zero. Players must rely on limited directional light and high-contrast cues to find their way.

🛠️ Technical Stack & Tools
Game Engine: Unity (LTS Version)

Programming Language: C# (C-Sharp)

Editor/IDE: Microsoft Visual Studio / VS Code

UI Framework: TextMeshPro for high-fidelity responsive text.

Assets: Unity Standard Assets for PBR textures and materials.

📐 Implementation Details
1. Lighting & Illumination
The game utilizes dynamic lighting to shift the mood between levels.

Directional Light: Simulates natural sunlight in Level 1. In Level 2, it is dimmed and tinted dark blue to simulate a night/horror aesthetic.

Ambient Lighting: For Level 2, ambient light was set to absolute black, removing general visibility and forcing the player to use specific light sources.

2. Texture Mapping (UV Tiling)
To ensure realism across large surfaces, we implemented custom UV Tiling (X:50, Y:50). This technique prevents the "stretching" effect common on large 3D planes, ensuring stone and wood textures repeat naturally.

3. Scene Management
The UnityEngine.SceneManagement API handles all state transitions. The LevelLoader.cs script manages the flow from the Main Menu → Level 1 → Level 2 → Victory Screen.