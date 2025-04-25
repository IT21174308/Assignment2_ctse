# Assignment2_ctse: CTSE Lecture Notes Chatbot

This project implements a simple chatbot using a Large Language Model (LLM) to answer questions based on the CTSE (Current Trends in Software Engineering) lecture notes. The chatbot is developed using the **LangChain** framework, **HuggingFace Transformers**, and **FAISS** for document retrieval.

## Features
- **Interactive Chatbot**: The chatbot answers questions related to CTSE lecture notes.
- **Document Processing**: Lecture notes are extracted from multiple PDFs and split into smaller chunks for better retrieval.
- **Question Answering**: Uses a fine-tuned LLM (`google/flan-t5-base`) to generate answers from the context of lecture notes.
- **Efficient Search**: Leveraging **FAISS** for fast retrieval of relevant document chunks


## How to Use

### 1. Clone the Repository
Clone the repository to your local machine:

```bash
git clone https://github.com/IT21174308/Assignment2_ctse.git
```

### 2. Download or Prepare Your Lecture Notes
- Add your CTSE lecture notes PDF files to the `ctse_lecture_notes` folder in the project directory.
- Alternatively, modify the script to point to the folder where your lecture notes are stored.

### 3. Install Dependencies
Before running the project, make sure to install the required dependencies. You can install them using `pip`:

Dependencies include:
`langchain`
`transformers`
`PyPDF2`
`faiss-cpu`
`torch`
`huggingface_hub`

### 4. Run the Jupyter Notebook
Open the `chatbot.ipynb` notebook in a Jupyter environment. You can use Jupyter Lab or Jupyter Notebook. To do this, run the following command in your terminal:

```bash
jupyter notebook chatbot.ipynb
````
### 5. Ask Questions
In the notebook, you'll find a section where you can input your questions in a designated text box or input field. The chatbot will process your query and generate an answer based on the content from the CTSE lecture notes.

Simply type your question and press Enter or click the button to submit it. The system will retrieve relevant information from the lecture notes and provide an answer.

Example:

- **Input**: "What are the key principles of Agile software development?"
- **Output**: The chatbot will return an answer based on the lecture notes that cover Agile principles.
