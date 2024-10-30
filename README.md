# **Tormented Game**
> *A psychological horror survival game set in a sinister psychiatric hospital.*

## **Game Description**

**Tormented** is a psychological horror survival game set in a foreboding psychiatric hospital. Players take on the role of a man who wakes up without memories in this dark place, facing the harsh reality of his captivity and a violent alternate personality of which he has no recollection. Throughout the game, the protagonist must uncover the truth behind his confinement and the dark experiments conducted within the hospital as he struggles for freedom and sanity.

## **Story**

In the heart of a disturbing psychiatric hospital, a man wakes up with no memory of how he arrived. Captured while his violent alter ego was in control, he faces the unsettling reality of his captivity and the existence of his other half, of which he has no memory.

As the game progresses, the protagonist is subjected to brutal experiments under the guise of scientific research. Trapped in a cycle of pain and confusion, he begins to find scattered notes revealing the scientists' dark goals. These notes not only shed light on his situation but also uncover the macabre practices taking place in the hospital. Each clue he discovers heightens his urgency to escape.

The game reaches its climax when, on the day of his escape, his other personality abruptly takes control, triggering a fierce confrontation with hospital staff. Upon finally achieving his freedom, the protagonist vows to destroy the horrors within the hospital, carrying with him the scars of his captivity and a commitment to end the institution that nearly erased his identity.

## **Game Mechanics**

### Game Start

The game begins on a start screen prompting players to press `S` to start. Then, an instructions screen provides context and basic game controls. After instructions, players are transported to the first narrative scene, establishing the game’s somber and mysterious tone.

### Controls

- **Movement:** Use arrow keys to move.
- **Shoot:** Aim with the mouse and shoot using the left mouse button.
- **Inventory:** Press `I` to access the notes inventory.
- **Pause Menu:** Press `ESC` to open or close the pause menu.

### Objective

The main objective is to uncover the truth behind your capture and escape the hospital. To achieve this, you’ll face enemies patrolling the dark hallways and collect notes that provide vital information for your escape.

### How to Play

1. **Exploration:** Move through the hospital's different settings, avoiding or fighting enemies while searching for clues and notes that help unravel the story.
2. **Combat:** Aim and shoot enemies with the mouse. Some enemies patrol specific areas, while others remain stationary in certain places.
3. **Note Collection:** Find and read notes scattered throughout the hospital to gain insights on how to escape and learn about the experiments being conducted.
4. **Inventory Management:** Use the inventory to review collected notes, which are essential to uncovering the story and planning your escape.
5. **Level Progression:** As you advance, you’ll encounter levels with different enemy setups and more notes to discover.

### Narrative Scenes

The game is divided into multiple scenes that alternate between combat and exploration and narrative scenes that provide story insights. These scenes include:

- **A Disturbing Awakening:** The protagonist wakes up in a dark room, unsure of how he got there.
- **Shadows of the Past:** As he advances, the protagonist begins to recall fragments of conversations and past events.
- **Echoes of Pain:** The protagonist realizes the brutality of the experiments and that his mind is being manipulated.
- **Visions and Realities:** Hallucinations blur with reality, and the protagonist must press on to uncover the truth.
- **The Edge of Sanity:** The line between sanity and madness grows thin, yet the protagonist finds strength to move forward.
- **The Truth Revealed:** The protagonist finally learns the truth behind his capture and decides to escape and destroy the hospital.

## **Key Features**

- **Psychological Horror Atmosphere:** The game creates an oppressive and tense environment where every shadow and sound heightens the feeling of unease.
- **Deep Narrative:** Through notes and context scenes, players uncover a complex and disturbing story.
- **Health System:** Both the player and enemies have a health system, adding a strategic element to combat.
- **Immersive Background Music:** The background music adds an extra layer of tension, keeping players on edge.
- **Level Progression:** Levels become progressively more challenging, with more enemies and notes to uncover.

## **Project Overview**

### Core Functionality

This project includes Unity scripts that manage core game elements, such as player health, shooting mechanics, note inventory control, collision handling, and level progression. The game uses Unity and C# to integrate immersive features and a complex narrative to create a deep and interactive experience.

- **Main Functionality**: Unity scripts to manage health, shooting, note inventory, collision interactions, and level progression.
- **Technologies Used**: Unity Engine, C#, Unity API.
- **Challenges**: Ensuring smooth gameplay by optimizing real-time events, including audio handling, enemy generation, and victory conditions.
- **Future Improvements**: Modularization and granular control of settings in Unity Inspector for easier customization.

## **Table of Contents**
1. [Scripts Overview](#scripts-overview)
2. [Installation and Execution](#installation-and-execution)
3. [License](#license)

## **Scripts Overview**

### **1. `AudioListenerManager`**
   - **Function**: Ensures there is only one `AudioListener` in the scene, adding one to the `GameObject` if needed.

### **2. `CollisionLogger`**
   - **Function**: Logs collision events to the console to aid in debugging, providing details of the colliding object.

### **3. `DamageDealer`**
   - **Function**: Inflicts continuous damage to the player while in collision with the object, controlling the damage interval.

### **4. `EnemyManager`**
   - **Function**: Manages enemy spawning at specific points in the scene at set intervals.

### **5. `EnemyShooter`**
   - **Function**: Configures enemy projectile shooting towards the player at timed intervals.

### **6. `GameAudioManager`**
   - **Function**: Manages persistent audio across scenes using a singleton pattern to avoid duplicates.

### **7. `GameOverUIManager`**
   - **Function**: Controls the Game Over UI, displaying results and allowing players to restart.

### **8. `HealthManager`**
   - **Function**: Manages the health of players and enemies, including death handling and game over conditions.

### **9. `InstructionsController`**
   - **Function**: Allows players to advance from the instructions scene to the narrative by pressing `C`.

### **10. `LevelProgression`**
   - **Function**: Manages level progression by checking if the player has met objectives to proceed.

### **11. `MainMenuController`**
   - **Function**: Controls the main menu, allowing players to start the game by pressing `S`.

### **12. `NarrativeSceneController`**
   - **Function**: Controls scene transitions in narratives, advancing with `C` and setting end conditions if it’s the final scene.

### **13. `Note`**
   - **Function**: Represents a collectible note in the game. When the player collects it, its content is stored and displayed.

### **14. `NoteInventory`**
   - **Function**: Manages the player’s collected notes inventory, including adding, retrieving, and resetting notes.

### **15. `NoteInventoryController`**
   - **Function**: Controls the display of the note inventory UI, allowing players to close it with `I`.

### **16. `NoteManager`**
   - **Function**: Manages note collection and display, showing individual notes or the full inventory and pausing the game when opened.

### **17. `NoteSceneController`**
   - **Function**: Controls the display of note content in the scene and allows closing with `X`.

### **18. `PatrolAndChase`**
   - **Function**: Sets up enemy patrol and chase behavior. Enemies patrol designated points and pursue the player within a specified range.

### **19. `PauseMenuController`**
   - **Function**: Controls the pause menu, allowing players to close it with `Escape` or restart the game with `Enter`.

### **20. `PauseMenuManager`**
   - **Function**: Manages the pause menu, opening or closing it with `Escape` and toggling the game state.

### **21. `PlayerMovement`**
   - **Function**: Manages player movement and toggles the notes inventory with `I`.

### **22. `PlayerShooter`**
   - **Function**: Allows the player to shoot projectiles towards the mouse cursor with the left mouse button.

### **23. `Projectile`**
   - **Function**: Controls projectile behavior, including movement and collision handling, dealing damage to the player or enemies as appropriate.

## **Installation and Execution**

1. **Prerequisites**:
   - **Unity 2021.3 or higher** - [Download Unity](https://unity.com/)

2. **Executing the Game**:
   - While the game build is available in `Build.zip` for local execution, playing directly via [itch.io](https://ivmg5.itch.io/tormented) is recommended for a seamless experience.
   - To run the build, extract `Build.zip` and open the executable (e.g.,

 `TormentedGame.exe`).

3. **Game Options**:
   - **In-Game Options**: Adjust settings and access the main menu to configure and progress through scenes.

## **License**

This project is licensed under the MIT License.

---

[![Build Status](https://img.shields.io/badge/status-active-brightgreen)](#)
[![Code Coverage](https://img.shields.io/badge/coverage-80%25-yellowgreen)](#)

---

Enjoy uncovering the secrets of **Tormented**, battling enemies and facing your inner demons to escape and expose the truth!

**Game Link: [Play on itch.io](https://ivmg5.itch.io/tormented)**
