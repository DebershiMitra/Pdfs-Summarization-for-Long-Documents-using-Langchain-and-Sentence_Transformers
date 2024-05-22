# Implementing-Extractive-and-Abstractive-Summarization-for-Long-Documents
Title: Implementing Extractive and Abstractive Summarization for Long Documents

# Introduction:
In this code implementation, we aim to summarize long documents using both extractive and abstractive techniques. Extractive summarization involves selecting important sentences directly from the text, while abstractive summarization involves generating new sentences that capture the essence of the document. We utilize Python libraries such as PyPDF2, Sumy, Transformers, and Langchain to achieve this goal.

# Code Breakdown:

Importing Libraries:
We import necessary libraries such as IPython.display, PyPDF2, sumy, langchain, transformers, and others to perform various tasks like display formatting, PDF processing, text summarization, and model loading.

Setting CSS:
A function set_css() is defined to set CSS for displaying code cells.

Installing Dependencies:
We install required packages like langchain, transformers, PyPDF2, and sumy using pip.

Login to Hugging Face Hub:
We log in to the Hugging Face Hub using an API token obtained from Google Colab userdata.

Extractive Summarization:
Text is extracted from a PDF document using the extract_text_from_pdf() function.
The extracted text is split into chunks using RecursiveCharacterTextSplitter.
Each chunk is summarized using the TextRank algorithm.
The final summary is printed.

Abstractive Summarization:
We initialize a BART model for abstractive summarization from the Hugging Face model hub.
The extracted summary from the extractive step is passed through the abstractive summarization model.
The abstractive summary is printed.

Abstractive Summarization (Alternate Approach):
An alternative approach for abstractive summarization is provided, using the BART model directly.
Text is preprocessed and chunked for input to the model.
The model generates a summary based on the input text chunks.
The summary is printed.

# Conclusion:
This code demonstrates a comprehensive approach to summarizing long documents using both extractive and abstractive methods. By combining these techniques, we aim to provide concise and informative summaries that capture the key points of the input document.
