**README.md for Barcode Label Generator**

## Overview

This Python script generates individual barcode labels in PDF format, suitable for thermal printers. Each label displays a barcode and its corresponding numeric value, retrieved from a provided Excel spreadsheet.

**Requirements**

- Python 3.x ([https://www.python.org/](https://www.python.org/))
- `openpyxl` library ([https://openpyxl.readthedocs.io/](https://openpyxl.readthedocs.io/))
- `reportlab` library ([https://www.reportlab.com/](https://www.reportlab.com/))

**Installation**

**Linux/macOS:**

1. Make sure you have Python 3 installed:
    - Check: `python3 --version`
    - Install: [https://www.python.org/downloads/](https://www.python.org/downloads/)
2. Install required libraries:
    ```bash
    pip install openpyxl reportlab
    ```

**Windows:**

1. Download and install Python 3: [https://www.python.org/downloads/](https://www.python.org/downloads/)
   - Choose the 32-bit or 64-bit installer based on your system.
   - During installation, check the option to "Add Python 3.x to PATH".
2. Open a command prompt or PowerShell window.
3. Install required libraries:
    ```
    pip install openpyxl reportlab
    ```

**Usage**

1. **Prepare your data:** Create an Excel spreadsheet named `barcodes.xlsx` with the barcodes' numeric values in column A.
2. **Download or clone the script:** Download the `barcodes.py` script from your repository or clone the entire repository.
3. **Place files together:** Ensure both `barcodes.xlsx` and `barcodes.py` are in the same directory.
4. **Run the script:** Open a terminal or command prompt in the directory containing both files and run:
    ```
    python barcodes.py
    ```

5. **Output:** The script will create a new directory named `Barcode_Pdfs` and generate individual PDF barcode labels within it. Each label will have a 60mm x 30mm dimension and contain the barcode along with the corresponding numeric value from the spreadsheet.

**Customization**

You can customize the following aspects of the script by modifying its source code:

- Label size (currently 60mm x 30mm)
- Barcode type (currently Code 128)
- Font size and style
- PDF filename pattern

**Additional Notes**

- This script is designed for thermal printers that can process PDF files directly.
- For non-thermal printers, you may need to use a PDF-to-image converter and send the images to your printer.

I hope this improved README.md file provides a clear and comprehensive guide for using your barcode label generator script!
