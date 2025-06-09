# Tic-Tac-Toe: Glitched Mode 🌀

This is a **modded version** of the classic Tic-Tac-Toe game built in C using the Raylib library and compiled for the web using Emscripten (EMSDK). This version introduces a chaotic twist: after each move, there's a **50% chance** that the move will **flip**—changing X to O or O to X—adding unpredictability and fun to the gameplay.

## 🧠 What's Unique?

- 🎲 **Flip Mechanic**: After placing a symbol, it may randomly switch to the opposite symbol.
- 🤖 **Play Against Computer**: Supports intelligent computer opponent using the **Minimax algorithm**.
- 👥 **Two Player Mode**: Play locally with another person—both players are affected by the glitch.
- 🎮 **Web-Compatible**: Play directly in your browser with no setup required.

## 🕹️ Features

- 3x3 Tic-Tac-Toe board.
- Clean graphical interface using Raylib.
- Glitch mechanic for added randomness.
- Two modes: Player vs Player and Player vs Computer.
- Lightweight and fast performance in web browsers.

## ⚙️ Tech Stack

- **C Programming Language**
- **Raylib** – For graphics and input handling.
- **Emscripten SDK (EMSDK)** – To compile C to WebAssembly for web deployment.
- **Minimax Algorithm** – For computer AI logic.

## 🚀 How to Play

Open the game in any modern browser:

👉 [Play the Game](https://alyoexe.github.io/tictactoe-moded/main.html)

## 🖥️ Local Development

If you want to build the project yourself:

1. Install [Raylib](https://www.raylib.com/)
2. Install [Emscripten](https://emscripten.org/docs/getting_started/downloads.html)
3. Compile with:

   ```bash
   emcc main.c -o index.html -s USE_GLFW=3 -s ASYNCIFY --shell-file shell.html -O2 -I/path/to/raylib/include -L/path/to/raylib/lib -lraylib
