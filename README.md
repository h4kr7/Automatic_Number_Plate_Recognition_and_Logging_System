# Vehicle License Plate Detection

This project utilizes OpenCV and Tesseract OCR to detect and recognize vehicle number plates in real-time using a webcam. Detected number plates are saved along with the timestamp in an Excel file.

## Features
- Real-time number plate detection using a webcam.
- Number plate recognition using Tesseract OCR.
- Saves detected number plates with timestamp in an Excel file.
- Supports multiple number plate formats.

## Supported Formats
The following formats are supported for number plate recognition:

- **Format**: 2 letters, 2 numbers, 2 letters, 4 numbers
- **Format**: 3 letters, 4 numbers
- **Format**: 2 letters, 2 numbers, 1 letter, 4 numbers
- **Format**: 2 numbers, 2 letters, 4 numbers, 1 letter

## Installation

1. **Install required libraries**:\
    Make sure you have Python installed.\
    You can install the required libraries using pip:
    ```bash
    pip install -r requirements.txt
    ```
2.  **Install Tesseract OCR**:\
    Download and install tesseract-ocr-w64-setup-5.4.0.20240606.exe\
    Update the path in the code:
    ```bash
    pytesseract.pytesseract.tesseract_cmd = r"C:\Program Files\Tesseract-OCR\tesseract.exe"
    ```
3. **Download Haar Cascade**:\
    Download haarcascade_russian_plate_number.xml\
    Ensure you have the haarcascade_russian_plate_number.xml file in the project directory.
