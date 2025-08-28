# BERT-based Document Classification

A system for classifying documents by extracting text from various file types using a BERT model.

---

## 🚀 About the Project

This project aims to solve the problem of unstructured data analysis by automatically classifying documents. It processes files like images and Word documents, extracts text using specialized libraries, and then uses a fine-tuned **BERT model** to classify the content into predefined categories. The main goal is to create an efficient and accurate document understanding system for various business and academic applications.

### Features:

- **Multimodal Input:** Processes both image files (.png, .jpg) and Word documents (.docx).
- **Text Extraction:** Uses Pytesseract for OCR on images and Textract for text retrieval from documents.
- **Sequence Classification:** Employs a BERT model trained on specific labels to categorize documents based on their textual content

## 🛠️ Getting Started

Follow these instructions to get a copy of the project up and running on your local machine.

### Prerequisites

Ensure you have the following software installed:

* `Python 3.8+`
* `tensorflow` or `keras`
* `Transformers`
* `Torch`
* `Pytesserac`
* `Textract`

### Installation

1.  Clone the repository:
    ```bash
    git clone [https://github.com/vinaykumartm1/Multimodal-System.git]
    ```
2.  Navigate to the project directory:
    ```bash
    cd Multimodal-System
    ```
### Usage

To run the main script and start the document classification process, execute the following command in your terminal:

 ```bash
    python Main.ipynb
  ```

### 📁 Data Processing

The read_data_from_folder function handles the data ingestion. It processes different file types:

**Images:** Handled using Pytesseract to perform Optical Character Recognition (OCR).

**Word Documents:** Processed using Textract for text extraction.

The extracted text is then tokenized using the BERT tokenizer to prepare it for the model.

### 🧠 Model Training

The BERT model is trained for sequence classification on a dataset with specified labels from a train.csv file. The training process uses the AdamW optimizer and runs for three epochs.

### 📈 Testing and Evaluation

The model's performance is evaluated using data from the test folder. The calculate_recall function computes recall scores for various fields, providing a clear measure of the model's accuracy in identifying specific information.

## 📈 Results

The final recall scores are printed to the console, showing the model's performance for key fields.

## 🔮 Future Work

This project provides a solid foundation, and there are many avenues for future development and improvement. Potential enhancements include:

- **Model Enhancements:** Explore more advanced transformer architectures like RoBERTa or Longformer for improved performance on long documents. Implement advanced hyperparameter tuning for a more optimized model.

- **Expanded File Support:** Extend the system to process a wider range of document formats, including PDFs, CSVs, and other common business document types.

- **Enhanced Evaluation:** Introduce a more comprehensive evaluation suite, including metrics like F1-score and a detailed confusion matrix, to better understand model performance.

- **Multilingual Support:** Adapt the system to handle documents in multiple languages by fine-tuning multilingual transformer models.



