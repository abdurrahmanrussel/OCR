## Bangla and English PDF OCR Extractor

This project provides a simple and efficient way to extract text from **scanned PDF documents** in both **Bangla (Bengali)** and **English** using **Google Colab**. It leverages Tesseract OCR and pdf2image to convert scanned PDF pages into readable text.

---

## 🚀 Features

* ✅ **Bangla PDF OCR** - Extracts text from Bangla PDFs.
* ✅ **English PDF OCR** - Extracts text from English PDFs.
* ✅ **Memory-Efficient** - Processes each page one by one, avoiding memory overflow.
* ✅ **High Accuracy** - Uses `dpi=300` for English and `dpi=150` for Bangla for clearer image conversion.
* ✅ **Downloadable Text File** - Extracted text is saved as `.txt` and can be downloaded easily.

---

## 📦 Dependencies

Run the following commands in **Google Colab**:

```bash
!pip install pytesseract pdf2image PyPDF2
!apt-get install -y poppler-utils tesseract-ocr tesseract-ocr-ben
```

For **English OCR**:

```bash
!pip install pytesseract pdf2image
!apt-get install -y poppler-utils tesseract-ocr
```

---

## 📌 Usage

### **1️⃣ Bangla PDF OCR Extraction**

```python
# ✅ Upload scanned Bangla PDF
from google.colab import files
uploaded = files.upload()
pdf_file = list(uploaded.keys())[0]

# ✅ Extract text and save it
!python bangla_pdf_ocr.py
```

### **2️⃣ English PDF OCR Extraction**

```python
# ✅ Upload scanned English PDF
from google.colab import files
uploaded = files.upload()
pdf_file = list(uploaded.keys())[0]

# ✅ Extract text and save it
!python english_pdf_ocr.py
```

---

## 📥 Output

* The extracted text will be saved as:

  * `bangla_book_full_ocr.txt` for Bangla OCR
  * `english_ocr_output.txt` for English OCR
* A download link will be provided to save it to your local machine.

---

## 🤝 Contributing

Contributions are welcome! Please fork this repository and create a pull request with your improvements.

---

## ✨ Author

Developed with ❤️ by [Md. Abdur Rahman](https://github.com/abdurrahmanrussel).

