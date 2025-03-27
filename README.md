# ArtiFrame

**ArtiFrame** is a real-time graphics application developed in C++ using openFrameworks. This project allows interactive manipulation of images and 3D models with a rich set of features including image import/export, vector drawing, scene transformation, camera control, texture mapping, and advanced illumination models.

## Table of Contents

- [Overview](#overview)
- [Features](#features)
- [Technologies](#technologies)
- [Installation & Compilation](#installation--compilation)
- [Usage](#usage)
- [Authors](#authors)

## Overview

ArtiFrame is designed for real-time image and model manipulation. The application is developed using **C++** along with libraries such as **OpenGL**, **openFrameworks**, and **ofxDatGui**. It provides both 2D and 3D functionalities with an intuitive user interface.

## Features

- **Image Processing**
  - Import and export images (PNG, JPEG, GIF)
  - Image sampling and color space adjustments (HSB/RGB)
  - Histogram display for selected images

- **Vector Drawing**
  - Automatic creation of primitives (square, rectangle, circle, ellipse, polygon)
  - Additional shapes such as stars and arrows
  - Dynamic cursor and transformation tools

- **3D Interactivity**
  - Real-time scene management using a hierarchical scene graph
  - Camera controls (movement, rotation, zoom, and reset)
  - Multiple light sources with adjustable illumination models (Lambert, Phong, Blinn-Phong)

- **Advanced Graphics**
  - Texture mapping with filtering and tone mapping options
  - Procedural texture generation using Perlin noise
  - Support for ray tracing including reflection, refraction, and global illumination

## Technologies

- **Language:** C++
- **Graphics Libraries:** OpenGL, openFrameworks
- **UI Library:** ofxDatGui
- **Development Environment:** Visual Studio 2022
- **Additional:** OpenMP for parallel processing

## Installation & Compilation

1. **Download the Repository:**
   - Clone or download the repository archive.

2. **Setup Dependencies:**
   - Ensure that [openFrameworks](https://openframeworks.cc/download/) is installed.
   - Install [ofxDatGui](https://github.com/braitsch/ofxDatGui) as an addon.
   - Copy the `ofxbraitsch` folder (or the relevant addon) into the `addons` directory of your openFrameworks installation.

3. **Project Generation:**
   - Navigate to the `projectGenerator` in openFrameworks.
   - Select the provided project folder.
   - Add required addons: `ofxAssimpModelLoader`, `ofxGui`, and `ofxDatGui`.
   - Choose Visual Studio 2022 as the development environment.
   - Click **Update** to generate the project files.

4. **Post-Generation Steps:**
   - Remove the auto-generated files (`ofApp.cpp` and `ofApp.h`) if necessary.
   - In Visual Studio, go to **Project Properties → C/C++ → Language** and enable OpenMP support (set to “Yes (/openmp)”).

5. **Build the Project:**
   - Open the solution in Visual Studio 2022 and build the project.

## Usage

- **2D Mode:**
  - Use keyboard shortcuts (e.g., `spacebar + i` for image import, `s` for drawing a square, `r` for a rectangle, etc.) to interact with the canvas.
  - Access transformation tools via the on-screen menu to move, rotate, or delete objects.

- **3D Mode:**
  - Navigate the scene using keys `W, A, S, D, Q, E` for movement.
  - Use mouse controls for camera rotation and zoom.
  - Double-click to reset the camera to its initial position.
  - Use numeric keys (1, 2, 3) to adjust light positions.

## Authors

- **Charles Brassard** – 536 783 602
- **Mathieu Chrétien** – 536 875 935
- **Vincent Cousineau** – 536 961 396
- **Anthony Veillet** – 536 779 403
