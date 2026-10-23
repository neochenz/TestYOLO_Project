# Project Roadmap: Gemma 4 & Robotics Simulation

## 1. Simulation Strategies
We have three levels of simulation planned to bridge the gap between AI logic and physical hardware:

### Level 1: Logic Mock (Fastest/Easiest)
* **Goal:** Test AI "vision" and decision-making logic.
* **Setup:** Python script + Webcam $\rightarrow$ Detect human $\rightarrow$ Print command to console (e.g., `[COMMAND]: STOP`).
* **Focus:** Software logic without hardware complexity.

### Level 2: Virtual Robot (Professional Simulation)
* **Goal:** Test AI interaction with physics and a 3D environment.
* **Setup:** Webots Simulator + Webcam injection $\rightarrow$ Virtual robot moves in 3D space based on real-world visual input.
* **Focus:** Spatial awareness and movement dynamics.

### Level 3: Hardware-in-the-Loop (Most Realistic)
* **Goal:** Full integration of AI, PC, and physical hardware.
* **Setup:** PC/Webcam $\rightarrow$ USB/Serial Communication $\rightarrow$ Arduino $\rightarrow$ SunFounder Mars Rover Kit motors.
* **Focus:** The "Nervous System" (communication between computer and electronics).

---

## 2. Current Environment State (Reference)
* **Primary Drive:** `F:` (All heavy tools and models are kept here to protect the C: drive).
* **Python Environment:** Miniconda located at `F:\Work_Dev\Tools\Miniconda3`.
* **Active Conda Env:** `gemma_sim` (Python 3.10).
* **Workspace Root:** `F:\Work_Dev\Projects\Gemma_Simulation`.
* **Model Cache:** `F:\Local_AI\Models\huggingface_cache` (via `HF_HOME`).
* **IDE:** VS Code Portable.

---

## 3. Vision Optimization (Future Planning)
* **Goal:** Optimize resource usage and processing speed.
* **Strategy:** Implement controls for webcam resolution and input stream binning to reduce computational load/cost.
* **Status:** Pending hardware availability (webcam).

---

## 4. Immediate Next Task: YOLO Deployment
**Project Folder:** `F:\Work_Dev\Projects\TestVOLO_Project`

**Objective:** 
Deploy a lightweight version of YOLO (You Only Look Once) to prepare the vision system. Even without a webcam currently available, we want to build and verify the code structure so it is ready for "plug-and-play" once hardware arrives.

**Steps for New Chat:**
1. Create the project directory.
2. Do not set up a new Conda environment unless necessary or missing. Update the current `gemma_sim` environment as the first priority.
3. Install necessary vision libraries (`ultralytics`, `opencv-python`).
4. Write a basic script to initialize the model and prepare for video stream input.
