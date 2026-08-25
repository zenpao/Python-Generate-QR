# Python-Generate-QR

A simple command-line Python tool for generating QR codes from any text or URL, as either a PNG or SVG file. The output file's folder path is automatically copied to your clipboard for quick access.

**A ready-to-use executable is available in [`/dist`](./dist) — no Python installation required.**

## Features

- Generate a QR code from any text/URL input
- Choose output format: **PNG** (common) or **SVG**
- Output filename is auto-generated with a timestamp (e.g. `QRCode_PNG_20250424120000000000.png`)
- Saves the file to the same folder the script is run from
- Automatically copies the output folder path to your clipboard for easy pasting into File Explorer

## Tech Stack

- **Python 3**
- [`qrcode`](https://pypi.org/project/qrcode/) `7.4.2`
- [`pyperclip`](https://pypi.org/project/pyperclip/) `1.9.0`
- [`DateTime`](https://pypi.org/project/DateTime/) `5.5`

## Prerequisites

- Python 3 (only needed if running from source — the packaged executable in `/dist` requires no Python installation)

## Installation

Clone the repository:

```bash
git clone https://github.com/paoradox/Python-Generate-QR.git
cd Python-Generate-QR
```

Install dependencies:

```bash
pip install -r requirements.txt
```

## Usage

### Option 1: Run from source

```bash
python generateQR.py
```

You'll be prompted to:
1. Choose an output type:
   - `P` — PNG QR code (common)
   - `V` — SVG QR code
   - `X` — Exit
2. Enter the text or URL to encode.

The QR code is saved in the same folder as the script, and its folder path is copied to your clipboard.

### Option 2: Run the packaged executable

A pre-built Windows executable, `run-generateQR.exe`, is available in [`/dist`](./dist) — run it directly, no Python installation required.

## Sample Output

A sample generated QR code is included at the repo root: `QRCode_PNG_SampleOutput.png`.

## Project Structure

```
Python-Generate-QR/
├── dist/
│   └── run-generateQR.exe        # Packaged Windows executable
├── generateQR.py                 # Main script
├── requirements.txt
├── QRCode_PNG_SampleOutput.png   # Sample generated output
└── ico.ico                       # App icon
```

## License

Not specified.
