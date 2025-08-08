# 🎮 Word Search Game — x86 Assembly ⌨️

### 📌 Description
This project is a fully functional, console-based Word Search game developed entirely in x86 Assembly language (MASM). I created this for my Computer Organization and Assembly Language (COAL) course to demonstrate a practical application of low-level programming. The game utilizes the Irvine32 library to interact with the Windows console for all input, output, and file handling.
Players are presented with a main menu and can play through three levels of increasing difficulty, with their score and lives tracked. The game also features a persistent high-score system and console color customization.

### 🎯 Objectives
- To apply fundamental x86 assembly concepts to build a complete, interactive application.
- To demonstrate proficiency with the MASM assembler and the Irvine32 library.
- To implement game logic, including state management, user input processing, and file I/O at a low level.
- To practice modular programming in assembly by structuring the code into distinct procedures for maintainability.

---
  
### 🧠 Gameplay — In a Nutshell
- The player is greeted with a main menu with options to Start Game, get Help, change Console Color, view the Highest Score, or Quit.
- The game consists of 3 levels. In each level, a grid of letters is displayed from a .txt file.
- The player must find the hidden words in the grid and enter them.
- If the word is correct, the score increases. If it's wrong, a life is lost.
- The goal is to find all the words in all three levels before running out of lives. The final score is then saved if it's a new high score.

---

### 🛠 Technologies & Concepts Used

| Component        | Description |
|------------------|-------------|
| **x86 Assembly (MASM)** | The primary language used for all game logic, memory management, and control flow. |
| **Irvine32 Library** | A crucial library that abstracts complex Win32 API calls for console I/O, file handling, and color control. |
| **Visual Studio 2022** | The IDE used for development, debugging, and project management. |
| **File I/O** | Reading level grids and instructions from .txt files, and writing the high score back to disk. |
| **Procedural Programming** | The code is structured into modular procedures (level1, read_file, changecolor, etc.) for clarity. |
| **String Manipulation** | Uses repe cmpsb for efficient comparison of the player's input against the list of correct words. |
| **Direct Memory Management** | All variables, arrays, and buffers are manually defined and manipulated in the .data segment. |

---

### 📁 File Structure

A clean repository is essential. This is the recommended file structure.

├── Project1.sln                  # Visual Studio Solution file (opens the project)<br>
├── Project1/<br>
│   ├── Project1.vcxproj          # Visual Studio Project file (build settings)<br>
│   ├── Project1.vcxproj.filters  # VS file filters<br>
│   ├── Text.asm                  # The main assembly source code!<br>
│   ├── level1.txt                # Data for level 1<br>
│   ├── level2.txt                # Data for level 2<br>
│   ├── level3.txt                # Data for level 3<br>
│   ├── instruction.txt           # The help/instructions text<br>
│   └── high_score.txt            # Stores the persistent high score<br>
├── screenshots/<br>
│   ├── menu.png                  # Screenshot of the main menu<br>
│   └── gameplay.png              # Screenshot of a level in progress<br>
└── README.md                     # You're reading it!```<br>
**Note:** A `.gitignore` file is used to exclude Visual Studio's temporary files (like the `.vs`, `Debug`, and `x64` folders) from the repository.

---

### 🖥️ Screenshots

**Main Menu**
<img width="1366" height="725" alt="menu" src="https://github.com/user-attachments/assets/9c810faf-d8b2-4b63-b2f9-986b8d30120d" />


**Gameplay in Action**
<img width="1366" height="721" alt="gameplay" src="https://github.com/user-attachments/assets/13791718-1d1f-4afc-b425-970c59ed81e4" />

---

### 📦 How to Set Up and Run

This project is designed for Windows and requires Visual Studio.

#### 🔧 Prerequisites
1.  **Visual Studio 2022** with the **"Desktop development with C++"** workload installed.
2.  During installation, ensure the **MASM component** is included.
3.  The **Irvine32 library** (`Irvine32.inc` and `Irvine32.lib`) must be set up for your project.

#### 🚀 Compile & Run
1.  **Clone** this repository to your local machine.
2.  Open the **`Project1.sln`** file in Visual Studio 2022.
3.  **Build** the solution (Press `F7` or go to `Build > Build Solution`).
4.  **Run** the project (Press `Ctrl+F5` or go to `Debug > Start Without Debugging`).

### 💡 Key Learnings
*   **Low-Level Control:** Gained a deep appreciation for how modern high-level languages handle memory, I/O, and program structure automatically.
*   **The Power of Assembly:** Understood the efficiency of specific instructions like `repe cmpsb` for tasks that would require loops in higher-level languages.
*   **System Interaction:** Learned how an application interfaces with the operating system (via the Irvine32 library's Win32 API calls) to perform tasks like reading files and writing to the console.
*   **Debugging Challenges:** Sharpened my debugging skills by using Visual Studio's debugger to inspect registers and memory, which is essential for assembly programming.

### 🧪 Tested On<br>

| OS          | Status                                                                    |
| ----------- | ------------------------------------------------------------------------- |
| ✅ **Windows 10/11** | ✔️ Fully Functional                                                   |
| ❌ **Linux/macOS** | ❌ Not supported (Depends on Windows-specific libraries and MASM) |

---

### 🙋‍♂️ Author
**Muhammad Ashir**  
Student of FAST-NUCES  
For contributions or queries, feel free to connect on LinkedIn [LinkedIn/ashir-qayyum](https://www.linkedin.com/in/ashir-qayyum)

### 📜 License
This project is licensed for educational and academic use. Attribution is appreciated.
