# Flash Game Launcher

A modern, dark-themed desktop application to organize and play your favorite `.swf` Flash games. Built with Python and PyQt6.

🇹🇷 *[Türkçe okumak için tıklayın (Read in Turkish)](README-TR.md)*

## Features

- **Modern UI**: A sleek dark theme with a responsive grid layout.
- **Auto-Detection**: Automatically scans the `swf_files` directory for any `.swf` files.
- **Game Thumbnails**: Automatically loads cover images for your games. Just place an image (e.g., `.png`, `.jpg`, `.webp`) with the exact same name as your `.swf` file in the `swf_files` directory.
- **Built-in Updater**: Features a fully automatic in-app self-updater. It checks GitHub for new releases, downloads the latest executable, seamlessly replaces the old one, and restarts automatically.
- **Standalone**: Easily packaged into a single standalone `.exe` using PyInstaller.

## How to Use

1. **Download the latest release**: Grab the latest `.exe` from the [Releases](../../releases) page.
2. **Setup your games**: 
   - Run the application once to automatically create the `swf_files` folder.
   - Place your Flash games (`.swf`) inside the `swf_files` folder.
   - (Optional) Place cover images with matching names inside the same folder (e.g., `super_mario.swf` and `super_mario.png`).
3. **Play**: Click the "Play" button on any game card. The launcher uses `FlashPlayer11.exe` to run the games asynchronously.

## Build from Source

### Prerequisites
- Python 3.10+
- `pip`

### Installation
1. Clone the repository:
   ```bash
   git clone https://github.com/BartuAbiHD/FlashGameLauncher.git
   cd FlashGameLauncher
   ```
2. Install the required dependencies:
   ```bash
   pip install -r requirements.txt
   ```
3. Run the application:
   ```bash
   python main.py
   ```

### Building the Executable
To build a standalone executable for Windows:
```bash
build.bat
```
This will create a `.venv`, install the dependencies, and use PyInstaller with the provided `main.spec` file to generate the `.exe`.

## License
© 2026 BartuAbiHD. All rights reserved.
