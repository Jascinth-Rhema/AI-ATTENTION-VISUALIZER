# AI Attention Visualizer

AI Attention Visualizer is a Streamlit-based application that helps visualize how attention is distributed across words in text extracted from an image.

The application combines OCR, text embeddings, and an attention mechanism to identify and display the words that receive higher attention scores.

## Features

- Upload an image containing text
- Extract text using OCR
- Process and clean extracted text
- Generate word embeddings
- Calculate attention scores
- Visualize attention for individual words
- Display the most attended word
- Interactive and user-friendly Streamlit interface
- Bright and animated UI

## How It Works

The application follows these steps:

```text
Image
  ↓
OCR
  ↓
Extracted Text
  ↓
Text Processing
  ↓
Word Embeddings
  ↓
Attention Calculation
  ↓
Attention Scores
  ↓
Visualization
````

## Technologies Used

* Python
* Streamlit
* NumPy
* Pillow
* Pytesseract
* Tesseract OCR
* Sentence Transformers
* PyTorch

## Project Structure

```text
AI-ATTENTION-VISUALIZER/
│
├── app.py
├── attention.py
├── embedding.py
├── ocr.py
├── requirements.txt
├── .gitignore
└── README.md
```

## File Description

### app.py

Main Streamlit application. It handles the user interface, image upload, text processing, attention calculation, and visualization.

### ocr.py

Extracts text from uploaded images using Tesseract OCR.

### embedding.py

Generates numerical vector representations of words using a sentence-transformer model.

### attention.py

Calculates attention scores for the extracted words.

### requirements.txt

Contains the Python packages required to run the project.

## Installation

### 1. Clone the Repository

```bash
git clone https://github.com/Jascinth-Rhema/AI-ATTENTION-VISUALIZER.git
```

### 2. Open the Project

```bash
cd AI-ATTENTION-VISUALIZER
```

### 3. Create a Virtual Environment

```bash
python -m venv .venv
```

### 4. Activate the Virtual Environment

Windows PowerShell:

```powershell
.\.venv\Scripts\activate
```

### 5. Install Python Dependencies

```bash
pip install -r requirements.txt
```

## Tesseract OCR Setup

This project uses Tesseract OCR for extracting text from images.

Install Tesseract OCR on Windows and make sure the Tesseract executable is available in the system PATH.

The common installation location is:

```text
C:\Program Files\Tesseract-OCR\tesseract.exe
```

If required, configure the Tesseract path in `ocr.py`.

## Run the Application

Start the Streamlit application using:

```bash
streamlit run app.py
```

The application will open in your browser.

## Example Workflow

1. Open the application.
2. Upload an image containing text.
3. The application extracts text using OCR.
4. The extracted text is processed into individual words.
5. Word embeddings are generated.
6. Attention scores are calculated.
7. Attention scores are displayed visually.
8. The word with the highest attention score is highlighted.

## Attention Mechanism

The project uses the concept of attention to calculate the importance of different words.

The standard scaled dot-product attention formula is:

```text
Attention(Q, K, V) =
softmax(QKᵀ / √dₖ)V
```

Where:

* Q = Query
* K = Key
* V = Value
* dₖ = Dimension of the key vectors

The calculated scores are used to visualize how attention is distributed across the extracted words.

## Use Cases

This project can be useful for understanding:

* Natural Language Processing
* Attention mechanisms
* Word embeddings
* OCR-based text processing
* AI and machine learning concepts
* Visualization of NLP models

## Future Improvements

* Support for multiple languages
* Better OCR preprocessing
* Interactive attention heatmaps
* Transformer-based attention visualization
* Sentence-level attention visualization
* Export attention results
* Support for PDF documents

## Author

**Jascinth Rhema R**

B.Sc Computer Science with Artificial Intelligence

## Repository

GitHub:
[https://github.com/Jascinth-Rhema/AI-ATTENTION-VISUALIZER](https://github.com/Jascinth-Rhema/AI-ATTENTION-VISUALIZER)

````



