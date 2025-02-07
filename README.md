# Rank Pack Creator - User Guide

## Overview
The Rank Pack Creator is a tool that allows users to generate a Minecraft resource pack with custom rank textures and Unicode mappings. Users can upload images, assign rank names, and export a properly structured resource pack.

---

## Prerequisites
Before using the tool, ensure you have the necessary dependencies installed.

### **Windows & Mac Requirements**
- Python (3.8 or later)
- Required Python libraries:
  ```sh
  pip install pillow tkinter
  ```
- Ensure you have a file explorer to browse for images.

---

## Installation & Setup
### **Windows**
1. Download and install Python from [python.org](https://www.python.org/downloads/).
2. Open **Command Prompt** and run:
   ```sh
   pip install pillow tkinter
   ```
3. Download or clone the Rank Pack Creator script.
4. Run the script by double-clicking or using:
   ```sh
   python rank_pack_creator.py
   ```

### **Mac**
1. Install Python via Homebrew if not installed:
   ```sh
   brew install python
   ```
2. Open **Terminal** and run:
   ```sh
   pip3 install pillow tkinter
   ```
3. Navigate to the script directory and execute:
   ```sh
   python3 rank_pack_creator.py
   ```

---

## How to Use the Rank Pack Creator
1. **Launch the Program**
   - Open the script via **Command Prompt (Windows)** or **Terminal (Mac)**.

2. **Upload Rank Images**
   - Click the "Upload Image" button.
   - Select a `.png` image (height must be **≤ 200px**).
   - Enter a rank name (**no spaces or uppercase letters**).

3. **Generate the Pack**
   - Click "Generate Pack" to create the resource pack.
   - Choose a folder to save your pack.
   - The program will automatically create `default.json` and `pack.mcmeta`.

4. **Locate the Unicode Mappings**
   - After generation, a `unicode_mappings.txt` file is created.
   - The file opens automatically, displaying Unicode characters for each rank.
   - You can manually open it from the saved directory.

5. **Using the Pack in Minecraft**
   - Move the generated `.zip` file to:
     - **Windows:** `%appdata%\.minecraft\resourcepacks`
     - **Mac:** `~/Library/Application Support/minecraft/resourcepacks`
   - Enable the pack in Minecraft under **Resource Packs**.

---

## Troubleshooting
### **Common Issues & Fixes**
| Issue | Solution |
|--------|----------|
| `ModuleNotFoundError: No module named 'PIL'` | Run `pip install pillow` |
| Images aren't saving | Ensure you're selecting a valid directory |
| Unicode appears with double backslashes | The script now ensures correct formatting |

---

## Support
If you encounter issues, ensure Python and dependencies are correctly installed. For further assistance, check the error messages or reinstall the dependencies.

Enjoy customizing your Minecraft ranks!

