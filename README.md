# Gesture Recognition Control for PowerPoint Presentation using Microsoft Kinect Sensor

<img width="400" alt="Screenshot 2024-09-09 at 20 36 26" src="https://github.com/user-attachments/assets/a7ccf8be-49a6-4c42-88bd-6d05e0035546"> <img width="418" alt="Screenshot 2024-09-09 at 20 46 36" src="https://github.com/user-attachments/assets/21a60c47-d1be-442c-afc8-497243e8e2bd">

---

## Project Overview

This project demonstrates a gesture recognition system to control Microsoft PowerPoint presentations using the Microsoft Kinect Sensor and C#, leveraging the Kinect SDK. The system allows presenters to control slides with intuitive hand gestures or voice commands, enabling touchless navigation without the need for keyboard or clickers.

## Table of Contents

- [Features](#features)
- [Project Structure](#project-structure)
- [Technology Stack](#technology-stack)
- [Requirements](#requirements)
- [Installation & Setup](#installation--setup)
- [Usage Instructions](#usage-instructions)
- [Gesture Controls](#gesture-controls)
- [Speech Recognition](#speech-recognition)
- [Limitations](#limitations)
- [Keywords](#keywords)
- [License](#license)

---

## Features

- **Gesture-based slide navigation:** Move forward or backward in a PowerPoint presentation by extending your right or left arm.
- **Real-time visual feedback:** Application window displays your tracked head and hand positions with animated circles.
- **Speech recognition:** Control the UI and visual feedback using voice commands.
- **Multi-application support:** Gestures send key events to any application, not limited to PowerPoint.
- **Easy setup and operation:** Simple requirements and step-by-step instructions.

---

## Project Structure

The repository contains the following key components:

- `src/` — Main application source code (C#)
- `bin/` — Compiled binaries after build
- `README.md` — Project documentation (this file)
- `Resources/` — Supporting files, assets, and images
- `.sln` / `.csproj` — Visual Studio solution/project files

*(Your actual directory structure may vary depending on how you organize your code.)*

---

## Technology Stack

- **Programming Language:** C#
- **Framework:** .NET Framework (Windows)
- **Hardware:** Microsoft Kinect Sensor (v1)
- **SDK:** Kinect for Windows SDK v1.7
- **Optional:** Microsoft Office PowerPoint (for controlling slides)

---

## Requirements

- Microsoft Kinect Sensor for Windows
- Kinect for Windows SDK v1.7
- Windows PC (compatible with Kinect SDK)
- Optional: Microsoft Office PowerPoint

---

## Installation & Setup

1. **Install the Kinect SDK:**
   - Download and install [Kinect for Windows SDK v1.7](https://www.microsoft.com/en-us/download/details.aspx?id=40278)
   - Plug in your Kinect Sensor and ensure it is recognized by Windows.

2. **Clone this repository:**
   ```bash
   git clone https://github.com/arnobt78/Gesture-Recognition-Control-Powerpoint-Presentation--Microsoft-Kinect-Sensor.git
   cd Gesture-Recognition-Control-Powerpoint-Presentation--Microsoft-Kinect-Sensor
   ```

3. **Open the project in Visual Studio:**
   - Open the `.sln` file from the root directory.

4. **Build the solution:**
   - Restore any missing NuGet packages if prompted.
   - Build the solution (`Build > Build Solution`).

5. **Run the application:**
   - Connect your Kinect sensor.
   - Set your PowerPoint presentation (optional).
   - Start the application from Visual Studio or by running the compiled binary.

---

## Usage Instructions

1. **Stand in front of Kinect:** Position yourself at least five feet away from the sensor.
2. **Track your movements:** The application window will display your image and three tracking circles (head, left hand, right hand).
3. **Control slides with gestures:**
   - **Right arm extended**: "Next Slide" (sends right arrow key)
   - **Left arm extended**: "Previous Slide" (sends left arrow key)
4. **Present your PowerPoint:** Make PowerPoint the foreground application. Gestures will control slide navigation.
5. **Visual feedback:** The ellipses grow and change color when your hand exceeds the threshold (45 centimeters from head). Only one gesture is activated at a time.

---

## Gesture Controls

- **Right Arm Out**: Advances to the next slide (`Right Arrow`)
- **Left Arm Out**: Moves to the previous slide (`Left Arrow`)
- **Gesture Activation:** Gesture triggers only when the hand moves beyond a certain threshold from the head position. Each gesture only fires once per activation.

> **Tip:** Gestures also work in other applications. For example, you can move the cursor in Notepad using gestures.

---

## Speech Recognition

The application supports the following voice commands:

- `computer show window`
- `computer hide window`
- `computer show circles`
- `computer hide circles`

*There is a four-second delay after the program starts before speech recognition is activated.*

---

## Limitations

1. **Embedded video activation:** Cannot start embedded videos in PowerPoint directly. Use animations to trigger videos with arrow keys.
2. **Gesture sensitivity:** Gestures are based on the distance between your head and hands. Unintended movements (e.g., bending down, stretching) may trigger gestures accidentally.
3. **Kinect SDK version:** Only works with Kinect SDK v1.7 (may not be compatible with newer hardware or SDKs).

---

## Keywords

`Gesture Recognition`, `Kinect`, `PowerPoint`, `C#`, `Kinect SDK`, `Human-Computer Interaction`, `Presentation Control`, `Speech Recognition`, `Touchless UI`, `Computer Vision`

---

## License

This project is for research and demonstration purposes. Please refer to the LICENSE file (if provided) for usage details.

---

*Screenshots:*

Look above

---
