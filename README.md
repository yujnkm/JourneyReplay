# Journey Replay: User Experience Playback Software for Wide-Area Outdoor Augmented Reality

**Journey Replay** is a specialized software tool designed for the in-depth analysis of user behavior in wide-area outdoor Mixed Reality (MR) and Augmented Reality (AR) environments.

In the field of Human-Computer Interaction (HCI), particularly in the burgeoning domain of MR, understanding *why* a user makes a certain decision is critical. It's not enough to just log *what* they did; we must be able to examine the full context of their actions to truly understand their experience. This software is built to bridge that gap.

Journey Replay provides a robust platform to **monitor, replay, and measure human behavior** from recorded sessions. It allows researchers and developers to visually step back into a user's session, to see what they saw, and to analyze their movements and interactions. This ability to replay and examine user behavior is crucial for evaluating key metrics like **cognitive load, user recall, spatial search patterns, and overall user experience** in complex, real-world settings.



new one:
In the field of Human-Computer Interaction (HCI), particularly in the burgeoning and complex domain of wide-area outdoor Mixed Reality (MR), understanding why a user makes a certain decision is a critical research challenge. It is no longer sufficient to just log what a user did—for instance, noting timestamps, GPS coordinates, or simple button presses. These quantitative logs lack the qualitative context of the user's environment and perception. To truly understand their experience, we must be able to examine the full context of their actions, their perceptions, and their environment. This software is built to bridge that exact gap, moving from simple data collection to true behavioral understanding.

Journey Replay provides a robust platform to monitor, replay, measure, and deeply analyze human behavior from comprehensive recorded sessions. It moves beyond simple data logs and allows researchers and developers to visually and spatially step back into a user's session. You can see precisely what they saw (their first-person point-of-view), where they were looking (eye-gaze), and how they moved through the world. This ability to reconstruct and examine the entire decision-making process is crucial for evaluating key and often elusive metrics. These include cognitive load, situational awareness, user recall of environmental information, spatial search patterns, and the holistic overall user experience in dynamic, real-world settings that are otherwise impossible to replicate in a lab.



## 🎥 Demo Video

You can watch a full demo of the project here:
[**Watch the Demo Video**](https://www.youtube.com/watch?v=dQw4w9WgXcQ)

## ⚙️ Installation and Setup

To get started, you will need to download both parts of the split archive. **Both files are required** to unzip the project correctly.

* `VisualizerV2.zip` (68.6 MB)
* `VisualizerV2.z01` (70.0 MB)

### Instructions

1.  Place both `VisualizerV2.zip` and `VisualizerV2.z01` in the same directory.
2.  Use an unzipping tool (like 7-Zip or WinRAR) to extract `VisualizerV2.zip`. The tool will automatically detect `VisualizerV2.z01` to combine and extract the full 140 MB project.
3.  **Important:** For ease of use, unzip the project directly to your Desktop. This will create a folder at the path `C:\User\[your user id]\Desktop\VisualizerV2` and will work with the software's default path settings, minimizing configuration.

### Project Files

After unzipping, your `VisualizerV2` folder will contain the following 6 files. You only need to interact with `Kirby2020.exe`.

![Project file structure](https://i.imgur.com/NpGVotVqMO.png)

* `Kirby2020_Data` (Folder)
* `MonoBleedingEdge` (Folder)
* `Kirby2020.exe` (The application you will run)
* `SJ00` (File - This is the demo user's tracking data)
* `UnityCrashHandler64` (Application)
* `UnityPlayer.dll` (File)

## 🚀 How to Run

1.  Navigate to your unzipped `VisualizerV2` folder.
2.  Double-click **`Kirby2020.exe`** to start the Journey Replay visualizer.
3.  Once the application is open, you will see an editable file path at the top of the window.
4.  By default, this path may be preset to the author's original path, for example: `C:\User\yujnkm\Desktop\VisualizerV2`
5.  You **must change** the author's user ID (e.g., `yujnkm`) to your own Windows user ID. If your user ID is `jdoe`, the correct path should be: `C:\User\jdoe\Desktop\VisualizerV2`.
6.  Once the path is correct, the software will automatically scan that directory, find the `SJ00` demo data file, and the playback of the developer's trial session will begin automatically.

## 🖥️ Features & UI Overview

The visualizer is split into two main windows for simultaneous analysis, plus a full-featured playback bar.

### ⏯️ Playback Control Bar

Located at the top, this bar gives you full control over the session replay:
* **Play/Pause Button:** Controls the playback.
* **Timeline:** A scrubbable timeline showing the full session length. You can click anywhere to jump to that moment or drag the marker to move back and forth.
* **Speed Slider:** Adjust the playback speed from 1x (real-time) up to 100x.
* **File Icon:** Shows `SJ00` to confirm you are viewing the author's demo tracking data.
* **Session Button:** Allows you to skip to the next session (e.g., the next search task) included in the data file.

### 👁️ Left Window (First-Person POV)

This window shows exactly what the user saw from their HoloLens or AR device—their "Point of View."
* **Red Ball:** This floating red ball indicates the user's **eye-gaze**, showing precisely where they were looking and paying attention at any given moment.
* **Controlled Yellow (Indicator):** This yellow indicator represents the user's click or answer, showing their real-time interaction response as it was recorded from the data.

### 🦅 Right Window (Spectator View)

This window is for inspecting the user's activity from an external, "bird's eye" or "spectator" perspective. You can toggle between different camera modes for the best vantage point.

* **Free View:** Click this button to fly around the scene freely using the mouse and keyboard (see controls below). This is ideal for inspecting the environment from any angle.
* **Top Down View:** An eagle's-eye view of the environment. In this mode:
    * **Drag** with the mouse to pan the map.
    * **Scroll** with the mouse wheel to zoom in and out.
* **Reset View:** If you get confused, sick, or lost in the 3D space, click this to return to the default spectator view.

#### Visual Indicators (in Spectator View)

* **3D Path Line:** This line is drawn in the environment to show the path the user walked. It is colored using a time-based `viridis` palette (robust for various forms of colorblindness) to show progress. The line changes color as time passes to show the oldest (start) and newest (current) points in the path.
* **Circle Dot:** Represents the user's head and position in the 3D space.
* **Square Frame:** This frame, which moves with the circle dot, represents the user's Field of View (FOV) and shows which direction they are looking.

## ⌨️ Mouse and Keyboard Controls

These controls are for navigating the **Right Window (Spectator View)**, primarily when you are in **"Free View" (Flythrough) mode**.

### Flythrough Mode

1.  Click and **hold the right mouse button** to enter Flythrough mode.
2.  While holding, use the following controls:
    * **Look:** Move your mouse.
    * **Move Forward/Backward:** `W` / `S`
    * **Move Left/Right:** `A` / `D`
    * **Move Up/Down:** `E` / `Q`
    * **Move Faster:** Hold `Shift` while moving.

### General Viewport Controls (3-Button Mouse)

These controls are available to help the inspector find the best angle and vantage point.

| Action | Control |
| :--- | :--- |
| **Pan** | Hold **Middle Mouse Button** + Drag |
| **Orbit** (Not in 2D mode) | Hold **`Alt`** + **Left-click** + Drag |
| **Zoom** | Use the **Scroll Wheel** (or `Alt` + Right-click + Drag) |
| **Change Speed** (Flythrough only) | Use the **Scroll Wheel** *while moving* |

## 🧩 Built on a Digital Twin Foundation

This playback software is made possible by two prerequisite open-source projects from the same author. These projects are responsible for generating the **high-fidelity, lightweight digital twin model** of the environment used in this replay.

Why is this important? Raw tracking data (like GPS coordinates or head-tracking logs) tells very little about the user's experience. It's just a line on a map.

By replaying this data *within* an accurate digital twin, you can see exactly what the user was looking at and seeing. This allows researchers to understand the **cause and effect** of user search patterns and behavioral reasoning, providing a complete picture of their interaction with the world.

## 🧩 Research 



## 🧩 Citaion 

![alt text](readme_fig/logo.png)
