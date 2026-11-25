# QR Code Creator
 
A simple desktop app built with Python and Tkinter that turns any text or link into a QR code. Type your text, pick a few options, and hit **Convert**. The QR code shows up right inside the window and is saved as an image.
 
The app follows your system theme (light or dark) using the [Sun Valley ttk theme](https://github.com/rdbende/Sun-Valley-ttk-theme).
 
## Features
 
- Generate a QR code from any text or URL
- Choose the **border** width and **size** (QR version)
- Choose the **fill colour** and **back colour**: blue, green, white or yellow
- Live preview of the QR code inside the window
- **Img clear** button to remove the preview
- Automatically follows your system's light/dark theme
## Requirements
 
- Python 3.8 or newer
- Libraries:
  - [`qrcode`](https://pypi.org/project/qrcode/) (with Pillow)
  - [`sv-ttk`](https://pypi.org/project/sv-ttk/)
  - [`darkdetect`](https://pypi.org/project/darkdetect/)
- `tkinter` (included with most Python installs; on some Linux distros install `python3-tk`)
## Installation
 
```bash
git clone https://github.com/Sudhir-090/qrcode6000.git
cd qrcode6000
pip install qrcode[pil] sv-ttk darkdetect
```
 
## Usage
 
```bash
python qrmaker.py
```
 
1. Type or paste your text or link into the **Input your text here** box.
2. Pick your options at the top:
   - **Border**: thickness of the empty margin around the QR code
   - **Size**: QR version (1 to 8). Higher versions can hold more data and look denser
   - **Fill colour**: colour of the QR pattern
   - **Back colour**: colour of the background
3. Click **Convert**. The QR code appears on the right.
4. Click **Img clear** to remove the preview.
> **Tip:** Fill and back colours should be different, otherwise the QR code will be invisible. Use a dark fill on a light background for the best scanning results.
 
> **Note:** Converting automatically saves the QR code as `ans.jpg` in the folder where you ran the program. Each new conversion overwrites the previous file, so rename or move it if you want to keep it.
 
## Project structure
 
```
.
├── qrmaker.py   # the whole app
└── README.md
```
 
## Built with
 
- [Tkinter](https://docs.python.org/3/library/tkinter.html), the GUI
- [qrcode](https://github.com/lincolnloop/python-qrcode), QR code generation
- [sv-ttk](https://github.com/rdbende/Sun-Valley-ttk-theme), modern theme
- [darkdetect](https://github.com/albertosottile/darkdetect), system theme detection
## Ideas for the future
 
- Choose the save location and file name
- Save as PNG
- More colour options (custom colour picker)
- A save/copy button for the generated image
## License
 
Free to use and modify. Add a license of your choice (for example MIT) if you want others to reuse it.
 
