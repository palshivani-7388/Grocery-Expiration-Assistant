# 🛒 Grocery Expiration Date Management using CrewAI & Ollama

An AI-powered multi-agent system that reads grocery information, searches for food shelf-life information from **StillTasty**, and estimates expiration dates using **CrewAI**, **Ollama (Llama 3.1)**, and **ChromaDB**.

## 📌 Project Overview

This project automates grocery expiration date estimation by combining AI agents with web-based food storage knowledge.

The application:

- Extracts grocery items
- Searches StillTasty for refrigerated shelf life
- Estimates expiration dates based on purchase date
- Uses local LLMs through Ollama (no OpenAI API required)

---

## 🚀 Features

- 🤖 Multi-Agent architecture using CrewAI
- 🦙 Local LLM powered by Ollama (Llama 3.1)
- 🌐 Searches StillTasty for food shelf-life information
- 📅 Estimates grocery expiration dates
- 💻 Runs completely locally without OpenAI API
- 🔍 Uses semantic search with ChromaDB embeddings

---

## 🛠️ Tech Stack

- Python
- CrewAI
- CrewAI Tools
- Ollama
- Llama 3.1
- ChromaDB
- BeautifulSoup4
- Requests

---

## 📂 Project Structure

```
Grocery-Expiration-Management/
│
├── grocery_management.ipynb
├── README.md
├── requirements.txt
└── sample_receipt.jpg (optional)
```

---

## ⚙️ Installation

### Clone the repository

```bash
git clone https://github.com/your-username/Grocery-Expiration-Management.git
cd Grocery-Expiration-Management
```

### Install dependencies

```bash
pip install -r requirements.txt
```

---

## Install Ollama

Download and install Ollama:

https://ollama.com/download

Pull the required models:

```bash
ollama pull llama3.1:8b
ollama pull nomic-embed-text
```

Start Ollama:

```bash
ollama serve
```

---

## ▶️ Run the Project

Open Jupyter Notebook:

```bash
jupyter notebook
```

Open:

```
grocery_management.ipynb
```

Run all cells.

---

## Workflow

```text
Input Grocery Items
        │
        ▼
CrewAI Agent
        │
        ▼
Search StillTasty
        │
        ▼
Retrieve Shelf Life
        │
        ▼
Estimate Expiration Date
        │
        ▼
Return Results
```

---

## Example

### Input

| Item | Purchase Date |
|------|---------------|
| Milk | 10 July 2025 |
| Eggs | 10 July 2025 |
| Yogurt | 10 July 2025 |

### Output

| Item | Shelf Life | Estimated Expiration |
|------|------------|----------------------|
| Milk | 7 Days | 17 July 2025 |
| Eggs | 3–5 Weeks | 31 July–14 Aug 2025 |
| Yogurt | 1–2 Weeks | 17–24 July 2025 |

---

## Future Improvements

- OCR-based receipt scanning
- Barcode detection
- Reminder notifications
- Mobile application
- Database integration
- Dashboard for grocery tracking

---

## Author

**Shivani Pal**

GitHub: https://github.com/your-username

---

## License

This project is developed for educational and learning purposes.
