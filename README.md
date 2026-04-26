# Project README

## Overview
This project is a simple C program that captures and reports keyboard and mouse input using custom libraries. The main functionality includes detecting when keys are pressed or released, as well as mouse button presses and releases.

## Features
- Captures keyboard events (key press and release)
- Captures mouse events (button press and release)

## Project Structure
```
Cmd_PongConsole/
├── build/              # .exe files produced by Main.c
├── src/                # source code
│   ├── Main.c          # Entry point
│   └── *.h             # stand alone Header-based C-files, without *.c files that implement it
├── Makefile.linux      # Linux Build configuration
├── Makefile.windows    # Windows Build configuration
├── Makefile.wine       # Wine Build configuration
└── README.md           # This file
```

### Prerequisites
- C/C++ Compiler and Debugger (GCC, Clang)
- Make utility
- Standard development tools

## Build & Run
The project supports building for Linux, Windows (using Wine), and WebAssembly.

### Building on Linux
To build the project on Linux:
```sh
cd Cmd_PongConsole/
make -f Makefile.linux all
```

To clean and rebuild:
```sh
make -f Makefile.linux clean
make -f Makefile.linux all
```

### Running on Linux
After building, you can run the executable using:
```sh
make -f Makefile.linux exe
```

### Building on Windows (using Wine)
To build the project on a Linux machine for Windows:
```sh
cd Cmd_PongConsole/
make -f Makefile.wine all
```

To clean and rebuild:
```sh
make -f Makefile.wine clean
make -f Makefile.wine all
```

### Running on Windows (using Wine)
After building, you can run the executable using:
```sh
make -f Makefile.wine exe
```

### Building for WebAssembly
To build the project for web assembly:
```sh
cd Cmd_PongConsole/
make -f Makefile.web all
```

To clean and rebuild:
```sh
make -f Makefile.web clean
make -f Makefile.web all
```

After building, you can run the executable using:
```sh
make -f Makefile.web exe
```

This will start a web server and allow you to access your application in a web browser.