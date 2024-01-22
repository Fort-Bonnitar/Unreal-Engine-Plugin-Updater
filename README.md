# Unreal Plugin Converter Readme

## Table of Contents
- [Unreal Plugin Converter](#unreal-plugin-converter)
- [Getting Started](#getting-started)
  * [Prerequisites](#prerequisites)
  * [Installation](#installation)
- [Usage](#usage)
  * [Setting Paths](#setting-paths)
  * [Conversion Process](#conversion-process)
- [Convert to Executable](#convert-to-executable)
  * [1. Install PyInstaller](#1-install-pyinstaller)
  * [2. Navigate to Your Script's Directory](#2-navigate-to-your-script-s-directory)
  * [3. Run PyInstaller](#3-run-pyinstaller)
  * [4. Locate the Executable](#4-locate-the-executable)
  * [5. Test the Executable](#5-test-the-executable)
  * [6. Run the Executable](#6-run-the-executable)
  * [Note:](#note-)
- [Additional Information](#additional-information)
- [Credits](#credits)

## Unreal Plugin Converter

The Unreal Plugin Converter tool is designed to simplify the conversion of Unreal Engine plugins through a user-friendly graphical interface (GUI). It streamlines the process of updating plugins to align with different Unreal Engine versions.

## Getting Started

### Prerequisites

Ensure the following prerequisites are met before using the tool:

- Python 3.x
- Tkinter
- PIL (Python Imaging Library)

### Installation

1. Clone or download the repository.

2. Install the required Python packages using the following command:

   ```bash
   pip install pillow
   ```

3. Run the tool using the following command:

   ```bash
   python gui.py
   ```

## Usage

### Setting Paths

1. Launch the GUI by running the script.

2. The interface provides input fields and buttons to set the paths required for the conversion process:

   - **Plugin Path**: Select the Unreal Engine plugin file (`.uplugin`).
   - **Target Version RunUAT.bat File**: Choose the RunUAT.bat file for the target Unreal Engine version.
   - **Output Folder Path**: Set the output folder where the converted plugin will be saved.

3. Click the corresponding buttons to select the necessary files:

   - **Select Plugin**: Choose the plugin file.
   - **Select RunUAT.bat File**: Choose the RunUAT.bat file.
   - **Select Output Folder**: Choose the output folder.

### Conversion Process

4. Once all paths are set, click the **Start Rebuild** button to initiate the conversion process.

5. A messagebox will indicate the completion of the rebuild. Check the command line for further details.

## Convert to Executable

To convert the Python script into an executable (.exe) file, follow these steps:

### 1. Install PyInstaller

If you haven't installed `pyinstaller` yet, you can do so using the following command:

```bash
pip install pyinstaller
```

### 2. Navigate to Your Script's Directory

Open a terminal and navigate to the directory where the Python script (`gui.py`) is located.

### 3. Run PyInstaller

Use the following command to run `pyinstaller` and create the executable:

```bash
pyinstaller --onefile gui.py
```

### 4. Locate the Executable

After the process is complete, navigate to the `dist` directory:

```bash
cd dist
```

You should find the executable file with the same name as the script but without the `.py` extension.

### 5. Test the Executable

Run the generated executable to test if it works as expected:

```bash
./gui.exe
```

### 6. Run the Executable

You can now run the standalone executable (`GUI.exe`) to others without requiring them to install Python or any dependencies.

Remember to include any necessary assets (like images) in the same directory as the executable if the script relies on them.

### Note:

- The generated executable may trigger antivirus warnings because it's an executable created from Python script. This is common and usually harmless.

These instructions assume you are using a Unix-like environment (Linux or macOS). If you are using Windows, the commands may be slightly different, and you can run them in the Command Prompt.

## Additional Information

- **How To Use**: Click the **Help** button to view instructions on using the tool. It provides step-by-step guidance on selecting files and starting the rebuild process.

## Credits

- This GUI was generated using [Tkinter Designer](https://github.com/ParthJadhav/Tkinter-Designer) by Parth Jadhav.
