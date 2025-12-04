# Persian OCR Extractor (Tkinter + Tesseract)

A simple desktop application for extracting Persian (Farsi) and English text from images using **Python**, **Tesseract OCR**, and a **Tkinter GUI**.

The app supports:

- 🖼 Selecting images (`.png`, `.jpg`, `.jpeg`)
- 🔍 Extracting text using Tesseract  
- 📋 Copy extracted text to clipboard  
- 💾 Save extracted text as `.txt`  
- 🌙 Dark mode UI  
- ❗ Friendly error messages

---

## 📦 Features

| Feature | Description |
|--------|-------------|
| 📁 Image Selection | Choose an image using file dialog |
| 🔤 OCR Extraction | Supports `fas` + `eng` |
| 📋 Copy Button | Copy recognized text to clipboard |
| 💾 Save Output | Save text as .txt |
| ⚠️ Error Handling | Clear, readable messages |

---

## 🏗 Requirements

### 🔹 1. Python Libraries

Install required packages:

```bash
pip install pillow pytesseract
```

### 🔹 2. Install Tesseract OCR

Download the Windows installer:

👉 https://github.com/UB-Mannheim/tesseract/wiki

Default installation path:

```
C:\Program Files\Tesseract-OCR\
```

Make sure this folder contains language files such as:

```
eng.traineddata
fas.traineddata
osd.traineddata
```

---

## 🔧 Configuration

If Tesseract is not auto-detected, set the path manually in Python:

```python
pytesseract.pytesseract.tesseract_cmd = r"C:\Program Files\Tesseract-OCR\tesseract.exe"
```

---

## ▶️ Running the Application

Run:

```bash
python main.py
```

---

## 📤 Creating an EXE (Optional)

If you'd like to generate a Windows executable:

```bash
pip install pyinstaller
pyinstaller --noconsole --onefile main.py
```

Your EXE will be inside:

```
dist/
```

---



## 🤝 Contributing

Pull requests and issues are welcome.

---

## 📄 License

MIT License.
