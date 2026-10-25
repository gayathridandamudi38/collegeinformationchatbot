# 🎓 College AI Chatbot

## 📌 Project Overview

The **College AI Chatbot** is an AI-powered chatbot designed to provide information about a college. The chatbot allows students and users to ask questions related to college information and receive relevant answers through an interactive web interface.

The project uses college-related PDF documents as the source of information. These documents are processed and converted into a **FAISS vector database**, which helps the chatbot retrieve relevant information when a user asks a question.

The chatbot is developed using **Python and Streamlit** and provides a simple and user-friendly interface for interacting with the system.

---

## 🎯 Objective

The main objective of this project is to develop an intelligent college information chatbot that can:

* Provide college-related information quickly
* Allow users to ask questions in natural language
* Retrieve relevant information from college documents
* Reduce the need for manually searching through PDF documents
* Provide an easy-to-use interface for students and users

---

## ✨ Features

* 🎓 College information chatbot
* 💬 Natural-language question input
* 📚 Uses college PDF documents as the knowledge source
* 🔎 Retrieves relevant information from the stored documents
* ⚡ FAISS-based vector search
* 🤖 AI-powered question answering
* 🌐 Streamlit web interface
* ⏳ Displays a loading message while generating an answer
* ⚠️ Displays a warning when no question is entered

---

## 🛠️ Technologies Used

* **Python**
* **Streamlit**
* **FAISS**
* **AI / Natural Language Processing**
* **PDF Documents**
* **Vector Database**

---

## 📂 Project Structure

```text
College-AI-Chatbot/
│
├── chatbot/
│   │
│   ├── data/
│   │   ├── college.pdf
│   │   ├── fee_structure.pdf
│   │   └── syllabus.pdf
│   │
│   ├── vectorstore/
│   │   ├── index.faiss
│   │   └── index.pkl
│   │
│   ├── app.py
│   ├── chatbot.py
│   ├── create_vector_db.py
│   ├── requirements.txt
│   └── README.md
```

---

## 📄 Data Files

The chatbot uses the following PDF documents as its knowledge source:

### `college.pdf`

Contains information related to the college.

### `fee_structure.pdf`

Contains information about the college fee structure.

### `syllabus.pdf`

Contains syllabus-related information.

These documents are stored inside the `data` folder.

---

## 🔎 Vector Database

The project contains a `vectorstore` folder with:

```text
vectorstore/
├── index.faiss
└── index.pkl
```

The PDF documents are processed and converted into vector representations. These vectors are stored using **FAISS**.

When a user asks a question, the chatbot searches the vector database for relevant information and uses the retrieved information to generate an answer.

---

## ⚙️ How the Project Works

The project works in the following steps:

```text
College PDF Documents
        ↓
Document Processing
        ↓
Create Vector Database
        ↓
FAISS Vector Store
        ↓
User Question
        ↓
Similarity Search
        ↓
Relevant Information
        ↓
AI Chatbot
        ↓
Answer
```

### Step 1: Collect College Documents

College-related information is stored in PDF files inside the `data` folder.

### Step 2: Create Vector Database

The `create_vector_db.py` file is used to process the documents and create the vector database.

The generated vector database is stored inside:

```text
vectorstore/
```

### Step 3: Ask a Question

The user enters a question through the Streamlit application.

For example:

```text
What courses are offered?
```

### Step 4: Retrieve Relevant Information

The chatbot searches the FAISS vector database to find information relevant to the question.

### Step 5: Generate the Answer

The chatbot uses the retrieved information to provide an answer to the user.

---

## 🖥️ Application Interface

The application is developed using **Streamlit**.

The main interface contains:

* 🎓 College AI Chatbot title
* 💬 Question input box
* 🔘 Ask button
* 🤖 Answer section

Users can enter questions such as:

```text
What courses are offered?
```

```text
What is the fee structure?
```

```text
What is the syllabus?
```

The chatbot then provides the relevant answer.

---

## 📌 Main Python Files

### `app.py`

`app.py` is the main Streamlit application.

It provides the user interface and accepts questions from the user.

The question is passed to the chatbot using the `ask_bot()` function.

### `chatbot.py`

`chatbot.py` contains the chatbot logic.

It processes the user's question and retrieves the relevant information needed to generate the answer.

### `create_vector_db.py`

This file is responsible for creating the vector database from the college PDF documents.

### `requirements.txt`

This file contains the Python libraries required to run the project.

---

## ⚙️ Installation

### 1. Clone the Repository

```bash
git clone <https://github.com/gayathridandamudi38/collegeinformationchatbot.git>
```

### 2. Open the Project Folder

```bash
cd College-AI-Chatbot
```

### 3. Install Required Libraries

```bash
pip install -r requirements.txt
```

---

## ▶️ Running the Project

After installing the required dependencies, run the Streamlit application:

```bash
streamlit run app.py
```

The application will open in your web browser.

---

## 🔄 Creating the Vector Database

If the vector database needs to be created again from the PDF documents, run:

```bash
python create_vector_db.py
```

This processes the documents available in the `data` folder and creates the vector database.

The generated files are stored in:

```text
vectorstore/
```

---

## 💡 Example Questions

Users can ask questions related to the available college information, such as:

* What courses are offered?
* What is the fee structure?
* What is the syllabus?
* Tell me about the college.
* What information is available about the college?
* What are the details mentioned in the college documents?

The chatbot's responses depend on the information available in the provided PDF documents.

---

## 🔮 Future Enhancements

The project can be improved by adding:

* 💬 Chat history
* 🎤 Voice-based questions
* 🌐 Multiple-language support
* 📱 Improved mobile interface
* 📚 More college documents
* 👨‍🎓 Student-specific information
* 📅 Academic calendar information
* 📢 College announcements and notifications
* 🔐 Student login system

---

## 🎯 Advantages

* Saves time when searching through college documents
* Provides quick access to college information
* Easy-to-use interface
* Uses document-based information retrieval
* Reduces the need for manual PDF searching
* Can be extended with additional college documents

---

## 👩‍💻 Author

**Gayathri Dandamudi**

B.Tech – Artificial Intelligence

---

## ⭐ Conclusion

The **College AI Chatbot** provides an efficient way for students and users to obtain college-related information through a conversational interface. By combining college PDF documents, vector search, FAISS, AI-based question answering, and Streamlit, the project provides a simple and interactive information-retrieval system.
