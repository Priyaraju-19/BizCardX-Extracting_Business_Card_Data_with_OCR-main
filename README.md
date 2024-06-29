
# Business Card Data Extraction with OCR

## Introduction

The Business Card Data Extraction project utilizes Optical Character Recognition (OCR) technology to extract key information from business cards. By leveraging machine learning and image processing techniques, the project aims to automate the process of capturing and digitizing contact details from scanned or photographed business cards.
Problem Statement: You have been tasked with developing a Streamlit application that allows users to upload an image of a business card and extract relevant information from it using easyOCR. The extracted information should include the company name, card holder name, designation, mobile number, email address, website URL, area, city, state, and pin code. The extracted information should then be displayed in the application's graphical user interface (GUI).

## Project Structure

- `data/`: Directory containing sample business card images for testing.
- `src/`: Source code for OCR preprocessing, text extraction, and data parsing.
- `notebooks/`: Jupyter notebooks for experimentation, data exploration, and visualization (if applicable).
- `results/`: Directory for storing extracted data, reports, and visualization outputs.
- `README.md`: This file.
- `requirements.txt`: List of dependencies needed to run the project.

## Setup

### Prerequisites

Ensure you have the following installed:

- Python 3.8+
- Tesseract OCR engine
- OpenCV (optional for image preprocessing)
- Git (optional for version control)

### Installation

1. Clone the repository:
    ```bash
    git clone https://github.com/yourusername/business-card-ocr.git
    cd business-card-ocr
    ```

2. Create a virtual environment:
    ```bash
    python3 -m venv venv
    source venv/bin/activate  # On Windows use `venv\Scripts\activate`
    ```

3. Install the required dependencies:
    ```bash
    pip install -r requirements.txt
    ```

4. Install Tesseract OCR:
    - For Linux:
      ```bash
      sudo apt-get install tesseract-ocr
      ```
    - For macOS:
      ```bash
      brew install tesseract
      ```
    - For Windows: Download and install from [Tesseract-OCR](https://github.com/tesseract-ocr/tesseract).

## Usage

### Data Extraction

Run the OCR extraction script on sample business card images:
```bash
python src/extract_data.py --image path/to/business_card.jpg
```

### Preprocessing and OCR

Preprocess images (optional) and apply OCR to extract text:
```bash
python src/preprocess_image.py --image path/to/business_card.jpg
python src/perform_ocr.py --image path/to/preprocessed_image.jpg
```
### Conclusion

The Business Card Data Extraction with OCR project has successfully developed a solution to automate the extraction of contact information from business cards using Optical Character Recognition (OCR) technology. By leveraging machine learning techniques and image processing algorithms, the project aimed to streamline the process of digitizing business card data and integrating it into digital databases or contact management systems.
