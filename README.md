# OCR-cv

This project implements an Optical Character Recognition (OCR) pipeline using Computer Vision techniques. It takes raw images as input — such as scanned documents, receipts, or printed forms — and extracts readable text through a structured four-stage pipeline: Image Pre-processing → Text Detection → Text Recognition → Restructuring.

## 📁 Project Structure
├── MNIST_Image_Recognition.ipynb   # Neural network for digit recognition (foundational model)
├── OCR_Pytesseract.ipynb           # Full OCR pipeline using Pytesseract
└── README.md


# How It Works
The pipeline follows these stages (as shown in the architecture diagram):
1. Image Pre-processing — Converts input images to grayscale, resizes, normalizes pixel values, and        applies bitwise transformations to improve contrast and clarity.
2. Text Detection — Locates regions of interest in the image where text is present.
3. Text Recognition — Uses Pytesseract (a Python wrapper for Google's Tesseract OCR engine) to read and    decode the detected text.
4. Restructuring — Formats and outputs the extracted text in a clean, readable form.

# Tech Stack
Python — Core language
Keras / TensorFlow — Neural network for digit recognition
NumPy / Matplotlib — Data manipulation and visualization
OpenCV (cv2) — Image processing and resizing
Pillow (PIL) — Image loading and format handling
Pytesseract — OCR text extraction engine
Tesseract OCR — Underlying OCR engine by Google

# Usage
For digit recognition:
1. Open MNIST_Image_Recognition.ipynb
2. Run all cells to train the model on MNIST data
3. Provide any 28×28 grayscale digit image and call model.predict() to get a prediction
