#Multimodal System

##Introduction

This project aims to develop a document understanding system using the BERT (Bidirectional Encoder Representations from Transformers) model for sequence classification. The system processes various file types, such as images and Word documents, extracting text data for further analysis. The primary goal is to train a BERT model to classify documents into relevant categories based on their content.


##Installation

pip install transformers torch pandas pytesseract textract

##Usage

python assignment_1.ipynb


##Dependencies

-Transformers
-Torch
-Pandas
-Pytesseract
-Textract


##Data Processing

The read_data_from_folder function processes files within the specified folders. Images are processed using Pytesseract, while Word documents are handled with Textract. Text data is tokenized using the BERT tokenizer.

##Model Training

The BERT model is trained using the specified labels from the 'train.csv' file. The training loop involves optimizing with the AdamW optimizer over three epochs.

##Testing and Evaluation

Testing involves processing data from the 'test' folder and evaluating the model's predictions. The calculate_recall function computes recall scores for each field, providing insights into the model's performance.


##Results

Results are printed, displaying recall scores for each field, including 'Agreement Value,' 'Agreement Start Date,' 'Agreement End Date,' 'Renewal Notice,' 'Party One,' and 'Party Two.'

