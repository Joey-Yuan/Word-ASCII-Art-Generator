# Word ASCII Art Generator

Turn any image into ASCII art using your own word or a density-mapped character set - now with a polished UI, live resizing, and export tools.

## Features
- Guided UI with a header and sidebar controls
- Import image or draw your own sketch, then generate ASCII with one click
- Word mode and Density mode character mapping
- Draw mode with brush controls (size +/-)
- Live size controls: Width and Height sliders
- Lock Aspect to preserve image proportions while resizing
- Text Density slider to make the output lighter or darker
- Zoom and Pan preview (scale and position) without regenerating text
- Save to .txt, Copy to clipboard, Clear

## Requirements
- Python 3.9+
- pygame
- Pillow (PIL)

## Install
On Windows PowerShell:

```powershell
pip install pygame Pillow
```

If you use a virtual environment, activate it first.

## Run

```powershell
# If your terminal is in the repo root folder:
python .\ascii_words-main\main.py

# Or cd into the folder first:
cd .\ascii_words-main
python .\main.py
```

## Usage
1) Type your word in the input field.
2) Toggle Image or Draw under the input field.
3) If Image: click "Import Image" and choose a picture. If Draw: sketch in the art panel, then click "Generate ASCII Art".
4) Adjust Width/Height and toggle Lock Aspect as needed.
5) Use Text Density to control how filled the output looks.
6) Use Zoom and X/Y Offset to frame the preview (preview only).
7) Save to .txt or Copy to clipboard.

Tip: Use simple sketches and images with clear light/dark contrast for best results.

## Controls
- Source: Image, Draw
- Buttons: Import Image, Generate ASCII Art, Save, Copy, Clear
- Mode: Word (uses your word), Dense (uses a gradient like @%#*+=-:. )
- Brush: - and + to change size (also [ and ] keys)
- Size: Width (10-200), Height (5-100)
- Lock Aspect: Keeps Width/Height tied to source image proportions
- Text Density: 0-100% (lower = lighter, higher = darker)
- Zoom: 50-300% (preview only)
- X Offset / Y Offset: Pan the preview inside the panel

Notes:
- Zoom and pan affect the preview only; saved/copied text is unchanged.
- Text Density changes the generated characters (affects save/copy output).
 - In Draw mode, use left mouse to draw; press C to clear.

## Troubleshooting
- ModuleNotFoundError: Install missing packages:
	- `pip install pygame Pillow`
- Tk file dialogs don't appear: Some IDEs suppress Tk windows; run from a system terminal.
- Performance: Very large Width/Height values can slow generation; try smaller sizes and use Zoom to upscale the preview.
- Empty or faint results: Increase Text Density or choose images with clearer contrast.

## License
MIT (or your preferred license)