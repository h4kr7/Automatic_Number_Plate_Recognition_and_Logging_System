# Automatic Number Plate Recognition and Logging System

This project leverages OpenCV and Tesseract OCR to automatically recognize vehicle license plates in real-time using a webcam. The recognized plates are saved to an Excel file with date and time information. Additionally, the system allows users to capture images of the detected plates.

## Features
- Real-time license plate detection from webcam feed.
- Support for multiple license plate formats using regular expressions.
- Logs recognized license plates with timestamps to an Excel file.
- Option to save images of captured license plates.

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

## Example of Detected Plates:
![Example of Detected Plates](https://github.com/h4kr7/Automatic_Number_Plate_Recognition_and_Logging_System/blob/main/Images/image1.png)
## Data Stored in Excel:
The detected license plate numbers, along with the current date and time, are logged into an Excel file.

![Data Stored in Excel](https://github.com/h4kr7/Automatic_Number_Plate_Recognition_and_Logging_System/blob/main/Images/image2.png)
